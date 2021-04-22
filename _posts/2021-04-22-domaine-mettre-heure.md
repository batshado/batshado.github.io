---
layout: post
title:  "Mettre son domaine à l'heure"
date:   2021-04-21 16:48:00 +0200
author: batshado
categories: [windows server]
---
#### A réaliser en admin sur le contrôleur principal du domaine :
{% highlight ruby %}
net stop w32time
w32tm /config /syncfromflags:manual /manualpeerlist:"pool.ntp.org"
w32tm /config /reliable:yes
net start w32time
w32tm /resync /force
w32tm /query /status
{% endhighlight %}

#### Et sur les postes clients pour forcer la synchronisation :
{% highlight ruby %}
w32tm /resync /nowait
{% endhighlight %}