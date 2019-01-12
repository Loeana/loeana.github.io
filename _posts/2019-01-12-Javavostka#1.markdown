---
layout: default
title:  "Javawostka #1"
date:   2016-02-12 17:50:00
categories: main
---

Taki mały potworek, na którego się ostatnio natknęłam:

{% highlight java %}
 InnerKokos k = new Kokos().new InnerKokos();
{% endhighlight %}

Przez chwilę zastanawiałam się na co ja właściwie patrzę - po czym mnie olśniło! To wywołanie konstruktora klasy wewnętrznej - jako, że InnerKokos jest klasą wewnętrzną nie-statyczną obiekty tej klasy muszą zostać utworzone w obrębie obiektów klasy nadrzędnej - w tym przypadku Kokos. 
Dopóki tego nie zobaczyłam nie przyszłoby mi do głowy, że można w ten sposób z zewnątrz wywołać konstruktor klasy wewnętrznej - oczywiście przy założeniu, że jest to klasa publiczna.
