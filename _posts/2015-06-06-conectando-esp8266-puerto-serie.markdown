---
layout: post
title:  "Conectando el ESP8266 al ordenador por el puerto serie"
date:   2015-06-06
---

Para conectar el ESP8266 al pc basta con conectar el conversor USB-serie (menos el pin de 5v) al chip y conectar los pines CHIP_EN a Vcc (3.3v) y el pin IO15 (mirando desde arriba el primero de la derecha) a tierra gnd.

La terminal que he usado es la GTKTerm. Vamos a conectar el ESP8266 al puerto /dev/ttyUSB0, por lo que habrá que darle permisos de ejecución:

{% highlight sh %}
sudo chmod 777 /dev/ttyUSBS0
{% endhighlight %}

La configuración que he usado es la siguiente:

<figure>
	<img src="{{ '/assets/img/gtkterm_config.png' | prepend: site.baseurl }}" alt=""> 
	<figcaption>Fig1. - Configuración gtkterm para ESP8266 ESP-201</figcaption>
</figure>



Más info: <a href="http://hanneslehmann.github.io/2014/12/ESP8266Module/">IoT - First Test of ESP8266 WiFi Module</a> 