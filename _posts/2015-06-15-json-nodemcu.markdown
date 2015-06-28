---
layout: post
title:  "Usando json en nodemcu"
date:   2015-06-15
---

Para manejar jsons en nodemcu podemos requerir la libería "cjson" que viene incluida en el framework

{% highlight lua %}
local json = require "cjson"
luaObject = json.decode("{\"json\": \"string\"}");
jsonString = json.encode(luaObject)
{% endhighlight %}
