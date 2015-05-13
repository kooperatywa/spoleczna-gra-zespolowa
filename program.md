---
layout: default
title: Program
permalink: /program/
klasa: program
menu: 2
---

##Program seminarium

Przewidujemy ok. 20 minut na każde wystąpienie oraz ok. 10 minut na dyskusję.

<table>
  <tbody>
  {% for wyklad in site.data.program %}
    <tr>
    <td>{{ wyklad.godzina }}</td>
    <td>{% if wyklad.prelegent %}<b>{{ wyklad.prelegent }}</b> – {% endif %}{{ wyklad.tytul }}</td>
    </tr>
  {% endfor %}
  </tbody>
</table>