# Ejercicios en Wollok

---
layout: default
ejercicios:
  - name: Multipepita
    github: wollok/multipepita
    classroom: https://classroom.github.com/a/983lTmoo
  - name: Empanadas Giménez
    github: wollok/polimorfismoEmpanadasGimenez
    classroom: https://classroom.github.com/a/aO_2yfqS
  - name: Cosas que le gustan a distintas personas
    github: wollok/objetosGustos
  - name: Viajes en auto
    github: wollok/viajesEnAuto
---

{% for ejercicio in page.ejercicios %}
  * {{ejercicio.name}} ([GitHub](https://github.com/{{ejercicio.github}}){% if ejercicio.classroom %} / [Classroom]({{ejercicio.classroom}}){% endif %})
{% endfor %}

<br>

Hay muchos más ejercicios para mirar en el [sitio GitHub de Wollok](https://github.com/wollok)
