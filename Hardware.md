---
layout: page
title: Hardware Designs
permalink: /hardware/
datatable: true
order_number: 5
---

#### Hardware designs of NIST PQC candidates

Here is a searchable and sortable list of optimised hardware designs of candidates to the NIST post-quantum standardisation project. To add your own results, please follow the instructions on the [About section](https://pqczoo.com/about/).

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
    <caption> </caption>

    <thead>
    {% for column in site.data.hardware[0] %}
        <th> {{ column[0] }} </th>
    {% endfor %}
    </thead>
    <tbody>
    {% for row in site.data.hardware %}
        <tr>
        {% for cell in row %}
            <td>{{ cell[1] }}</td>
        {% endfor %}
        </tr>
    {% endfor %}
    </tbody>
</table>
