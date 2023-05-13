# Microsoft 365 (Office 365) profile editor
A simple application what allow Microsoft 365 users to edit their own profiles

**All details about this app described in [my blog post](https://borisov.cloud/2023/05/13/how-to-allow-microsoft-365-office-365-users-to-update-their-own-profile/)**

Also you can run application as docker container using commands bellow


## Command to build docker image:
```
docker build --pull --rm -f "Dockerfile" -t yourimagetag:latest "."
```

## Command to run docker image with variables needed:
```
docker run -p 50000:50000 -e CLIENT_ID="<your app client id>" -e CLIENT_SECRET="<your app secret>" -e TENANT_NAME="<your tenant name or id>" yourimagetag:latest
```