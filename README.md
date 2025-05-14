# Spring Cloud Config Server & Client Implementation
## Overview

This is a demo application to show how we can externalize spring boot config property/yaml files and retrieve based on active profiles.

## Project Structure

This is a multi-module Spring boot application which has config-server and config-client modules. The application configuration is read from a public config-repo repository in github.

This repo contains 3 folders (dev, test and prod) and each have the config files (application.yaml and config-client.yaml). 

We have 2 config files just to show that any config file with the spring-application-name has more precedence when the config server searches the folder.

![config-repo-structure-1](https://github.com/user-attachments/assets/6928a51f-c820-4fb3-a1aa-bb00fc7cc8b0)

## Instruction to run application

- Clone Project
- Change the git uri in spring cloud config server application.yaml to a public git-repo you have created with the above folder structure.
- You can also use mine as it is publicly accessible -> https://github.com/olumide1128/config-repo
- Run the config-server application
- Change spring.profiles.active in config-client application.yaml to any profile you want to read config values from (dev,test or prod)
- Run the config-client application
- If all works well, once the config-client starts up, you should see an appropriate message in the console based on what profile you specified.


