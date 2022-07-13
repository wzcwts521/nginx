# podman init machine. Due to the current version of podman don't have default volume can be mounted on the host. 
```
podman machine init -v $HOME:$HOME
```
# build image


# podman cleanup unusage (dangling image)
```
podman image prune
```
 


# run image
podman run -d --rm --name test01 -v $(PWD)/customconf.d:/etc/nginx/customconf.d -p 0.0.0.0:8081:80 nginxcustom