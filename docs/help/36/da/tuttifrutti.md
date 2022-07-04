---
layout: print
title: Tutti
---

 
    {% for entry in site.data.navigation %}
 
        {% assign sublinks = entry.sublinks %}
        {% if sublinks %}
            
<h2>{{ entry.title }}</h2>
            
            {% for sublink in sublinks %}
                {% include_relative  {{ sublink.url }}.md %}
      
            {% endfor %}
  
 
        {% else %}
         
        {% endif %}
    {% endfor %}
    
 


