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