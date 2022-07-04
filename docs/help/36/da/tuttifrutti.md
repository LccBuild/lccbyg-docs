---
layout: print
title: Tutti
---

 
    {% for entry in site.data.navigation %}
 
        {% assign sublinks = entry.sublinks %}
        {% if sublinks %}
<p>---------------------------------------------------------------------------------------</p>            
<h2>{{ entry.title }}</h2>
            
            {% for sublink in sublinks %}
                {% include_relative  {{ sublink.url }}.md %}
      
            {% endfor %}
  
 
        {% else %}
          {% include_relative  {{ entry.url }}.md %}
        {% endif %}
    {% endfor %}
    
 


