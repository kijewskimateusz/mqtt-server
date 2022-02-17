# eclipse-MQTT server

login and password for server user:
```commandline
user: hass
password: hass
```

To change login and password, change password using commands below: (bash)
```commandline
sudo docker exec -it mqtt sh
mosquitto_passwd -c /mosquitto/config/pwfile {{login}}
{{password}}
{{repeat password}}
exit
```

Docker-compose command:
```commandline
docker-compose -p eclipse-mosquitto -f docker-compose.yml -f example.docker-compose.dev.yml up -d
```

Git checkout to latest release tag: 
```commandline
git fetch --all --tags

Fetching origin
From git-repository
   98a14be..7a9ad7f  master     -> origin/master
 * [new tag]         v1.0       -> v1.0
```

```commandline
git checkout tags/<tag> -b <branch>

Switched to a new branch 'v1.0-branch'
```
[Source](https://devconnected.com/how-to-checkout-git-tags/)