{% capture fecha %}{% assign d = semana.entrega.fecha | date: "%-w" | minus: 1 %}{{ site.data.fechas.dias[d] }} {{ semana.entrega.fecha | date: "%-d de " }}{% assign m = semana.entrega.fecha | date: "%-m" | minus: 1 %}{{ site.data.fechas.meses[m] }}{% endcapture %}