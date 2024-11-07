---

layout: lccbyghelp40  
title: "Rækkedetaljer"  
date: "2024-01-14"  

---

En række har, alt efter type forskellige sektioner der kan tilrettes.
De forskellige sektioner er:

{% capture included_file %}{% include_relative rowsettings.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative acquire.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative nonrecurringcost.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative maintain.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative restore.md %}{% endcapture %}
{{ included_file | split: "---" | last }}
 
{% capture included_file %}{% include_relative manage.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative cleaning.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative supply.md %}{% endcapture %}
{{ included_file | split: "---" | last }}

{% capture included_file %}{% include_relative income.md %}{% endcapture %}
{{ included_file | split: "---" | last }}
 
{% capture included_file %}{% include_relative nonrecurringincome.md %}{% endcapture %}
{{ included_file | split: "---" | last }}
 


.
