<h2>Research Projects by Topic</h2>

<ul>
 	<li><a href="projects/offpolicy.html">Off-policy policy evaluation</a></li>
 	<li><a href="projects/stepsizes.html">Stepsize selection</a></li>
</ul>

<h2>Publications by Year</h2>

<!-- Super important: do not indent the content line, because then it -->
<!-- gets treated like code -->
{% assign sortedyrs = (site.publications | sort: 'name') | reverse %}
{% for pubyr in sortedyrs %}

<h3>{{ pubyr.name }}</h3>

{{ pubyr.content | markdownify }}

{% endfor %}

