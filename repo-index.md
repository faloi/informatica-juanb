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
    classroom: https://classroom.github.com/a/iQjzZW_g
  - name: Viajes en auto
    github: wollok/viajesEnAuto
    classroom: https://classroom.github.com/a/vYA0wLuw
  - name: Spa
    github: wollok/spa
    classroom: https://classroom.github.com/a/Ai0icdEv
  - name: Sueldo de Pepe
    github: wollok/polimorfismoSueldoDePepe
    classroom: https://classroom.github.com/a/Wntnv_vc
  - name: Juego con personajes y elementos
    github: wollok/juegoPersonajesElementos
    classroom: https://classroom.github.com/a/PZm1ETWq
  - name: Casa de Pepe y Julián
    github: obj1-unahur/casaDePepeYJulian
    classroom: https://classroom.github.com/a/waLnAp4R
  - name: Juego interactivo con Pepita
    github: wollok/pepitaGame
    classroom: https://classroom.github.com/a/7jFBW_sF
---
[volver al inicio](./index.md)  

# Ejercicios en Wollok

{% for ejercicio in page.ejercicios %}
  * {{ejercicio.name}} ([GitHub](https://github.com/{{ejercicio.github}}){% if ejercicio.classroom %} / [Classroom]({{ejercicio.classroom}}){% endif %})
{% endfor %}

<br>

Hay muchos más ejercicios para mirar en el [sitio GitHub de Wollok](https://github.com/wollok)

# Wollok Game

En Wollok existe una herramienta visual para mostrar objetos, llamada Wollok Game. Eventualmente con ella se podrían hacer pequeños juegos, de ahí su nombre.

Si quieren investigar sobre esto les recomendamos que empiecen con [este ejemplo de Pepita](https://github.com/wollok/pepitaGame/tree/demoFirstClass). En el README del repositorio explica cómo hacerlo andar.
