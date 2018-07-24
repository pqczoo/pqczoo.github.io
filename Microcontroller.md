---
layout: page
title: Microcontroller Designs
permalink: /microcontroller/
datatable: true
---


<head>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
</head>

<link rel="stylesheet" type="text/css" href="https://cdn.datatables.net/1.10.19/css/jquery.dataTables.css">
  
<script type="text/javascript" charset="utf8" src="https://cdn.datatables.net/1.10.19/js/jquery.dataTables.js"></script>

<script src="/js/jquery.dataTables.js"></script>

<script src="/js/jquery.dataTables.min.js"></script>

<script>

$(document).ready(function() {
    $('#example').DataTable( {
        paging: true,
        order: [ 3, 'desc' ],
        stateSave: true,
        searching: true
    } );
} );

</script>

<table id="example" class="display" style="compact">
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
