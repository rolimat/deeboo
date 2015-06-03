---
layout: post
title:  "Solucionando el problema de las tildes en Sublime Text con Ubuntu"
date:   2015-06-02
---

Suelo usar bastante Sublime Text para el trabajo (aunque utilizo Intellij IDEA como IDE principal) y sobre todo en mis proyectos personales. El tema de las tildes es un poco problemático y en mi caso tras instalar Sublime no puedo escribir correctamente las tildes encima de las vocales.

Para solucionar este problema basta con agregar al fichero de configuración <b>Default (Linux).sublime-keymap</b> el código que se muestra más abajo. Para ello, hay que ir a "Preferences -> Key Bindings - User "


{% highlight xml %}
[

	// Remapeado de teclas de Sublime Text para teclado español en Ubuntu
	 
	// - á - Á
	{ "keys": ["´","a"], "command": "insert", "args": {"characters": "á"}},
	{ "keys": ["´","A"], "command": "insert", "args": {"characters": "Á"}},

	// - é - É
	{ "keys": ["´","e"], "command": "insert", "args": {"characters": "é"}},
	{ "keys": ["´","E"], "command": "insert", "args": {"characters": "É"}},

	// -í - Í
	{ "keys": ["´","i"], "command": "insert", "args": {"characters": "í"}},
	{ "keys": ["´","I"], "command": "insert", "args": {"characters": "Í"}},

	// - ó - Ó
	{ "keys": ["´","o"], "command": "insert", "args": {"characters": "ó"}},
	{ "keys": ["´","O"], "command": "insert", "args": {"characters": "Ó"}},

	// - ú - ü - Ú - Ü
	{ "keys": ["´","u"], "command": "insert", "args": {"characters": "ú"}},
	{ "keys": ["¨","u"], "command": "insert", "args": {"characters": "ü"}}, 
	{ "keys": ["´","U"], "command": "insert", "args": {"characters": "Ú"}},
	{ "keys": ["¨","U"], "command": "insert", "args": {"characters": "Ü"}},

]
{% endhighlight %}

Más info: <a href="" target="_blank">https://github.com/jesusabad/Tildes-en-vocales-para-Sublime-Text</a>