# mosquitto

Custom mosquitto image

Without authentication
```
docker run --rm -it --net=host mqtt
```

With authentication
```
docker run --rm -it --net=host mqtt sh -c "mosquitto_passwd -b /etc/mosquitto/passwd user user123; mosquitto -c /etc/mosquitto/conf.d/custom.conf"
```
