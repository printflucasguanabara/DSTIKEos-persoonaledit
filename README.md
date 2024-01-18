
Platform.io is configured and can be run e.g.
```shell
$ pio run -t upload && pio device monitor -p /dev/ttyUSB0 -f esp8266_exception_decoder
```

You'll notice that `Configuration.h` contains a wifi connection array this can be defined in the `PLATFORMIO_BUILD_FLAGS` environment variable e.g.
```shell
$ PLATFORMIO_BUILD_FLAGS="'-DWIFI_SSID=\"my-ssid\"' '-DWIFI_PASS=\"my-password\"'" \
pio run -t upload && pio device monitor -p /dev/ttyUSB0 -f esp8266_exception_decoder
```
