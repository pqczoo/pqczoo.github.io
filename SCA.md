---
layout: page
title: Side-Channel Analysis
permalink: /sca/
---

INSERT DESCRIPTION
.

.
.

.
.

.
.

.
.



{% assign mydata=site.data.foo %}

<table>
    <caption>Table caption</caption>
    <thead>
    {% for column in site.data.members[0] %}
        <th>{{ column[0] }}</th>
    {% endfor %}
    </thead>
    <tbody>
    {% for row in site.data.members %}
        <tr>
        {% for cell in row %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>
