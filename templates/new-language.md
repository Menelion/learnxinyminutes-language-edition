---
author: {YOUR_NAME}
layout: default
permalink: /{LANG_CODE_1}-{LANG_CODE_2}
tags: {LANG_CODE_1} {LANG_CODE_2} {LANG_NAME_1} {LANG_NAME_2}
title: {LANG_NAME_1} to {LANG_NAME_2}
sections: basics
---

# {LANG_NAME_1} to {LANG_NAME_2}

{% assign lang-code = page.url | replace: "/" %}
{% include translations.html %}
