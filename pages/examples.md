---
title: Example Entries
layout: page
permalink: /examples/
---

# Example entries

These entries come from the earlier virtual pilgrimage project. They are retained as examples of the project’s format and comparative method.

They are **not part of the current Amsterdam route**. Some locations, themes, and comparisons may differ from the requirements of the current course project.

## Why we include examples

Example entries show how a location, a Middle English passage, and a contemporary comparison can be brought together. They may also illustrate approaches that current entries develop, revise, or replace.

## Browse the examples

{% assign example_entries = site.examples | sort: "title" %}
<ul>
  {% for entry in example_entries %}
    <li>
      <a href="{{ entry.url | relative_url }}">{{ entry.title }}</a>
      {% if entry.categories %}
        <br />
        <small>{{ entry.categories | join: " · " }}</small>
      {% endif %}
    </li>
  {% endfor %}
</ul>

[Return to the current route](/)
