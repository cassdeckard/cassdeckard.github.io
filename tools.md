---
title: projects
description: things i have been working on
---

This page showcases how to list items in a specific collection.

<ul>
    {% for project in site.projects %}
        <li>
            <h2>
                <a href="{{ project.url | relative_url }}">
                    {{ project.title }}
                </a>
            </h2>

            <p>
                <i>{{ project.description }}</i>
            </p>
            <p>{{ project.excerpt }}</p>
        </li>
    {% endfor %}
</ul>
