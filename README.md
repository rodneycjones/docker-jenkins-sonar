# Docker, Jenkins, Sonar

## 1. Pre-requisites

To use this program, you must have `docker` and `docker-compose` installed on your computer. The installation process can be found on the [official Docker website](https://www.docker.com/)

## 2. Start the program

Go to the `jenkins` directory. Execute the following command. 

```Bash 
chmod 777 jenkins.sh
```

The command will give the rights to the container to execute the file `jenkins.sh`.

Now, you can start the program via the following command:

```Bash
docker-compose up
```

## 3. Jenkins and Sonar

Jenkins and Sonar are available on the following ports:

- Jenkins: 8080
- SonarQube: 9000

At the first start, Jenkins will ask you for a password. This password is displayed in the log. However, you can have access to this password via the container. 

To create a connection to the container, you have just to do this command:
```Bash 
docker exec -i -t jenkins bash
```
Use the command cat on the specific file and copy the password.

