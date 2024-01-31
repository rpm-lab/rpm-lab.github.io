---
title: "RPM Lab - Publications"
layout: gridlay
excerpt: "RPM Lab -- Publications."
sitemap: false
permalink: /publications/
---


## Publications

### 2024

<table cellspacing=10 style='font-family:"Arial", Courier, monospace; font-size:15px'>

<tr>
	<td>
		<center><img src='{{ site.url }}{{ site.baseurl }}/images/publications/slotGNN_Rezazadeh_et_al_arXiv_2023.png' width=250></center>
		
	</td>
	<td>
		Alireza Rezazadeh, Athreyi Badithela, <b>Karthik Desingh</b>, Changhyun Choi<br/>
		<i>"SlotGNN: Unsupervised Discovery of Multi-Object Representations and Visual Dynamics,"</i><br/>
		<b>Accepted ICRA 2024.</b><br/>
		[<a href='{{ site.url }}{{ site.baseurl }}/assets/bibs/rezazadeh2023SlotGNNarxiv'>Bibtex</a>] &nbsp;
		[<a href='https://arxiv.org/pdf/2310.04617.pdf'>Arxiv</a>] &nbsp;
		[<a href='https://www.youtube.com/watch?v=0fZBY5bMh3Q'>Video</a>] &nbsp;
		[<a href='https://www.alireza.page/slot-gnn'>Project page</a>] &nbsp;
		
	</td>
</tr>


<tr>
	<td>
		<center><img src='{{ site.url }}{{ site.baseurl }}/images/publications/geom_peg_Ku_et_al_arXiv_2023.jpeg' width=250></center>
		
	</td>
	<td>
		Chahyon Ku, Carl Winge, Ryan Diaz, Wentao Yuan, <b>Karthik Desingh</b><br/>
		<i>"Evaluating Robustness of Visual Representations for Object Assembly Task Requiring Spatio-Geometrical Reasoning,"</i><br/>
		<b>Accepted ICRA 2024.</b><br/>
		[<a href='{{ site.url }}{{ site.baseurl }}/assets/bibs/ku2023GeomPegarxiv'>Bibtex</a>] &nbsp;
		[<a href='https://arxiv.org/pdf/2310.09943.pdf'>Arxiv</a>] &nbsp;
		[<a href='https://www.youtube.com/watch?v=3e5QKCdmb7Q'>Video</a>] &nbsp;
		[<a href='https://sites.google.com/view/geometric-peg-in-hole/home'>Project page</a>] &nbsp;
		
	</td>
</tr>
</table>

<!-- ## Group highlights

**At the end of this page, you can find the [full list of publications and patents](#full-list-of-publications). All papers are also available on [arXiv](https://arxiv.org/search/?searchtype=author&query=Allan%2C+M+P).**

{% assign number_printed = 0 %}
{% for publi in site.data.publist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if publi.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <pubtit>{{ publi.title }}</pubtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ publi.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ publi.description }}</p>
  <p><em>{{ publi.authors }}</em></p>
  <p><strong><a href="{{ publi.link.url }}">{{ publi.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ publi.news1 }}</strong></p>
  <p> {{ publi.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>


## Patents
<em>Milan P Allan, S Gröblacher, RA Norte, M Leeuwenhoek</em><br />Novel atomic force microscopy probes with phononic crystals<br /> PCT/NL20-20/050797 (2020)

<em>Milan P Allan</em><br /> Methods of manufacturing superconductor and phononic elements <br /> <a href="https://patents.google.com/patent/US10439125B2/en?inventor=Milan+ALLAN&oq=inventor:(Milan+ALLAN)">US10439125B2 (2016)</a> -->

### Full List of publications

Please refer to [Karthik Desingh's list of publications](https://karthikdesingh.com/#pubs) for publications before 2024.


<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

{% for publi in site.data.publist %}

  {{ publi.title }} <br />
  <em>{{ publi.authors }} </em><br /><a href="{{ publi.link.url }}">{{ publi.link.display }}</a>

{% endfor %}
