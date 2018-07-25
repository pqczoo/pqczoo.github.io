---
layout: page
title: News

---

Any updates from the table will appear as a news item here, linked to a Twitter page.

<!-----add latest updates at the top ---->

- Side-channel analysis
	- Albrecht, M, Paterson, K & Deo, R, 2018, 'Cold Boot Attacks on Ring and Module LWE Keys Under the NTT', TCHES, vol 2018, no. 3.

<br/>

- Hardware designs
	- Howe, J, Tobias, O, Krausz, M, Güneysu, T, 2018, 'Standard Lattice-Based Key Encapsulation on Embedded Devices', TCHES, vol 2018, no. 3.

<br/>

- Microcontroller designs
	- Howe, J, Tobias, O, Krausz, M, Güneysu, T, 2018, 'Standard Lattice-Based Key Encapsulation on Embedded Devices', TCHES, vol 2018, no. 3.

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>
