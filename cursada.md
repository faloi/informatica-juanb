---
layout: default
---
# Semana a semana

{% assign semanas = site.data.semanas | sort %}
{% for semana_hash in semanas reversed %}
{% assign numero_semana = semana_hash[0] %}
{% assign semana = semana_hash[1] %}

## Semana {{numero_semana}}
{{semana.descripcion}}

{% if semana.ejercicios %}
### Ejercicios para trabajar en clase
<table>
    <thead>
        <tr class="header">
            <th>Nombre</th>
            <th>GitHub Classroom</th>
            <th>Repositorio original</th>
        </tr>
    </thead>
    <tbody>
      {% for ej in semana.ejercicios %}
      <tr>
          <td markdown="span">{{ej.name}}</td>
          <td markdown="span">[Clonar el ejercicio]({{ej.classroom}}) <i class="fas fa-book"></i></td>
          <td markdown="span">[Ver repositorio](https://github.com/{{ej.repo}}) <i class="fab fa-github"></i></td>
      </tr>
      {% endfor %}
    </tbody>
</table>
{% endif %}

{% if semana.mumuki %}
### Mumuki

Te recomendamos resolver las guías:
{% for guia in semana.mumuki %}
* [{{guia.nombre}}]({{guia.url}})
{% endfor %}
{% endif %}

{% if semana.entrega %}
### Para entregar

{% include obtener-fecha.md %}
La fecha límite para la entrega de esta semana es el **{{fecha}}**.

{% endif %}

{% if forloop.last == false %}
<hr class="titulo-semana">
{% endif %}

{% endfor %}
