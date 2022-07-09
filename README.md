# docker-flutter

Con esta imagen acoplable, no necesita instalar Flutter y SDK de Android en su máquina de desarrollador. Todo está listo para usar incluido un dispositivo emulador (Pixel con Android 9). Con un alias de shell, no reconocerá la diferencia entre la imagen y una instalación local. 

### Linux #2, Windows & MacOS (using host emulator)

Inicie su emulador de Android local. Luego, vuelva a conectar y ejecute el siguiente comando para que sea accesible a través de la red:

```shell
adb tcpip 5555
```
En su contenedor acoplable, conéctese al dispositivo:

```shell
adb connect host.docker.internal:5555
```

Ahora puede elegir el dispositivo para comenzar a depurar.