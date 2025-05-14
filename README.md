# Spring Cloud Config Server & Client Implementation
## Overview

This is a demo application to show how we can externalize spring boot config property/yaml files and retrieve based on active profiles.

## Proect Structure

This is a multi-module Spring boot application which has config-server and config-client modules. The application configuration is read from a public config-repo repository in github.

This repo contains 3 folders (dev, test and prod) and each have the config files (application.yaml and config-client.yaml). 

We have 2 config files just to show that any config file with the spring-application-name has more precedence when the config server searches the folder.

![config-repo-structure-1](https://github.com/user-attachments/assets/6928a51f-c820-4fb3-a1aa-bb00fc7cc8b0)

## Instruction to run application


