# EXERCISE 1.9 - VOLUMES

## Open Terminal

``` bash
touch text.log
docker run -v "$(pwd)/text.log:/usr/src/app/text.log" devopsdockeruh/simple-web-service
```
