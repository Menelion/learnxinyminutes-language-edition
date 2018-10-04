---
layout: default
---

# Learn X in Y Minutes (Language Edition)

Select your language to the language you want to learn.

Language Combinations: {{site.languages | size}}

{% for language in site.languages %}
  <h2>
     <a href="{{ language.url | prepend: site.baseurl }}">{{ language.title }}</a>
  </h2>
{% endfor %}
