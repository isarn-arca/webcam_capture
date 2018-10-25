# webcam_capture_MPlayer

**Selecionamos el dispositivo**
```bash
$ ls -ltr /dev/video*
```


**Instalamos el MPlayer (capturador de imagenes y videos)**
`$ sudo apt install mplayer`

**Ejecutamos el MPlayer para iniciar nuestra webcam (podemos pulsarla barra de espacio para pausar la imagen)**

`$ mplayer tv:// -tv driver=v4l2:width=640:height=480:device=/dev/video0 -fps 30`

**Pulsamos la tecla "s" para capturar una imagen**

`$ mplayer tv:// -tv driver=v4l2:width=640:height=480:device=/dev/video0 -fps 15 -vf screenshot`



# webcam_capture_guvcview-brlin

**Instalamos el Guvcview-Brlin (capturador de imagenes y videos y EDITOR)**
`$ sudo apt install guvcview`


**Ejecutamos Guvcview**
`$ sudo guvcview`

Se nos abrirá una ventana con el output de la webcam y otra con una interfaz para editar nuestra imagen variando diversos parametros


**IMPORTANTE: hay que asegurarse de haber instalado previamente las siguientes librerias**
`$sudo apt-get install cmake`
`$sudo apt-get install libopencv-dev`

## Tips
https://wiki.archlinux.org/index.php/webcam_setup

http://www.linuxintro.org/wiki/Set_up_a_Webcam_with_Linux

https://www.youtube.com/watch?v=kE_khSGn6H4
