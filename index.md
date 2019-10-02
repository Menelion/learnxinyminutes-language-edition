---
layout: default
title: Home
---

# Learn X in Y Minutes (Language Edition) [WORK IN PROGRESS]

Select your language to the language you want to learn.

Language Combinations: {{site.languages | size}}

{% assign languages = site.languages | sort: 'title' %}
{% for language in languages %}

## [{{language.title}}]({{ language.url | prepend: site.baseurl }})

{% endfor %}

## How to Contribute

[I want to contribute!](https://github.com/wboka/learnxinyminutes-language-edition/blob/master/.github/contributing.md)

### Contributors

A BIG thank you to the following contributors.

|       | Contributor | Contributions |
| :---: | ----------- | ------------: |
{% for contributor in site.github.contributors -%}

| <img src="{{contributor.avatar_url}}" alt="{{contributor.login}}'s avatar" width="32" height="32" /> | [{{ contributor.login }}]({{ contributor.html_url}}) | {{contributor.contributions}} |
{% endfor %}

### Do you see a language combination missing?

Copy one of the three templates below and add the missing information with a pull request (see below). Please keep sections separate: numbers in one file and greetings in another under the two letter code pattern that exists.

JSON

<pre>{% include_relative _data/templates/template-json.json %}</pre>

CSV

<pre>{% include_relative _data/templates/template-csv.csv %}</pre>

YAML or YML

<pre>{% include_relative _data/templates/template-yml.yml %}</pre>

### Do you see something missing from the existing languages?

Create a fork of this project and make the changes you want to see on the language combination specfic branch.

### Pull Requests

Please DO NOT send pull requests for multiple language combinations, it will be rejected.
