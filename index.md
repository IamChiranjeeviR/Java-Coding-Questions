---
layout: default
title: Java Questions
---

# 📚 Java Practice Questions

<ul>

{% raw %}
{% assign folders = site.static_files %}

{% for file in folders %}

    {% if file.path contains '/README.md' %}

        <li>
            <a href="{{ file.path }}">
                {{ file.path }}
            </a>
        </li>

    {% endif %}

{% endfor %}
{% endraw %}

</ul>
