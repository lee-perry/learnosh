---
layout: default
title: NGC1 | Element 1 - Foundations in health and safety
tipue_search_active: true
---

<table class="table">
  <thead class="thead-light">
    <tr>
      <th scope="col" colspan="4">Element 1: Foundations in health and safety</th>
    </tr>
  </thead>
  <tbody>
    
    {% assign sorted = site.pages | sort:"Unit" %}
      {% for page in sorted %}
   
        {% if page.module == 'NGC1' %}
          {% if page.Element == 1 %}

    <tr>
      <th scope="row">{{ page.Element }}.{{ page.Unit }}</th>
      <td><a href="{{page.url}}">{{ page.title}}</a></td>
      <td>v.{{ page.v }}</td>
      <td>{{  page.updated  }}</td>
        </tr>
          {% endif %}
        {% endif %}
      {% endfor %}

  </tbody>
</table>
