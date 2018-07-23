---
layout: page
title: Microcontroller Designs
permalink: /microcontroller/
datatable: true
---

<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<script type="text/javascript" src="js.min/bootstrap-table.min.js"></script>
<script type="text/javascript" src="js.min/Chart.bundle.min.js"></script>
<script type="text/javascript" src="js.min/datatable.min.js"></script>
<link rel="stylesheet" href="css.min/bootstrap-table.min.css">
<link rel="stylesheet" href="css.min/datatable.min.css">

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


{% assign mydata=site.data.microcontrollers %}

<table class="table database"
       data-id-field="Authors"
       data-sort-name="PQC Type"
       data-sort-order="desc"
       data-show-chart="false"
       data-pagination="false"
       data-show-pagination-switch="false">
    <caption>Table caption</caption>

    <thead>
    {% for column in site.data.microcontrollers[0] %}
        <th> {{ column[0] }} </th>
    {% endfor %}
    </thead>
    <tbody>
    {% for row in site.data.microcontrollers %}
        <tr>
        {% for cell in row %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>
