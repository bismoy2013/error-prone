---
title: Bug Patterns
layout: master
---

# Bug patterns

This list is auto-generated from our sources. Each bug pattern includes code
examples of both positive and negative cases; these examples are used in our
regression test suite.

Patterns which are marked __Experimental__ will not be evaluated against your
code, unless you specifically configure error-prone. The default checks are
marked __On by default__, and each release promotes some experimental checks
after we've vetted them against Google's codebase.

{% for maturity in site.data.bugpatterns %}

<h2>{{ maturity[0] }}</h2>
{% for pattern in maturity[1] %}
__<a href="bugpattern/{{pattern.name}}">{{pattern.name}}</a>__<br/>
{{pattern.summary}}
{% endfor %}

{% endfor %}