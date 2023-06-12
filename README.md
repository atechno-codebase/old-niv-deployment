# Old NIV deployment

## Running locally

 - Generate `personal access token` for your github account. Follow steps mentioned in [Github Documentation](https://docs.github.com/en/enterprise-server@3.4/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

 - Login to Github Container Registry:

 ```
 echo <your-personal-access-token> | docker login ghcr.io -u <your-github-username> --password-stdin

 ```

 - Run the services and dependencies locally:

 ```
 docker-compose up -d
 ```


## Debugging

 - Logs can be seen when services are started using command

 ```
 docker-compose up
 ```

 - If detached mode flag `-d` is used, then the container logs can be watched by running:

 ```
 docker logs <container-name>
 ```
