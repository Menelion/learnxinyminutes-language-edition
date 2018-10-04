---
layout: default
title: Home
---

# Learn X in Y Minutes (Language Edition) [WORK IN PROGRESS]

Select your language to the language you want to learn.

Language Combinations: {{site.languages | size}}

{% for language in site.languages %}
  <h2>
     <a href="{{ language.url | prepend: site.baseurl }}">{{ language.title }}</a>
  </h2>
{% endfor %}

### How to Contribute

#### Do you see a language combination missing?

Copy one of the three templates below and add the missing information with a pull request (see below). Please keep sections separate: numbers in one file and greetings in another under the two letter code pattern that exists.

JSON
<pre>{% include_relative _data/templates/template-json.json %}</pre>

CSV
<pre>{% include_relative _data/templates/template-csv.csv %}</pre>

YAML or YML
<pre>{% include_relative _data/templates/template-yml.yml %}</pre>

#### Do you see something missing from the existing languages?

Create a fork of this project and make the changes you want to see on the language combination specfic branch.

#### Pull Requests

Please DO NOT send pull requests for multiple language combinations, it will be rejected.
