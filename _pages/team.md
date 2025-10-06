---
title: "RPM Lab - Team"
layout: gridlay
excerpt: "RPM Lab: Team members"
sitemap: false
permalink: /team/
---

## Group Members

 <!-- **We are  looking for new PhD students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!** -->

<!-- Jump to [staff](#staff), [Ph.D. students](#master-and-bachelor-students) and [master and bachelor students](#master-and-bachelor-students). -->

<!-- Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors). -->

### Director
<div class="row team-grid">
{% for member in site.data.team_members %}
  <div class="col-xs-12 col-sm-6 col-md-4">
    <div class="team-card">
      {% if member.photo %}
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}"
           alt="{{ member.name }}" class="team-photo">
      {% endif %}
      <div class="team-body">
        <h4 class="team-name">{{ member.name }}</h4>
        {% if member.info %}<p class="team-role"><em>{{ member.info }}</em></p>{% endif %}
        {% if member.web %}<p><a href="{{ member.web }}" target="_blank">Home page</a></p>{% endif %}
        {% if member.number_educ %}
        <ul class="team-edu">
          {% for i in (1..member.number_educ) %}
            <li>{{ member['education' | append: i] }}</li>
          {% endfor %}
        </ul>
        {% endif %}
      </div>
    </div>
  </div>
{% endfor %}
</div>



### Ph.D. Students
<div class="row team-grid">
{% for member in site.data.phd_students %}
  <div class="col-xs-12 col-sm-6 col-md-4">
    <div class="team-card">
      {% if member.photo %}
      <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}"
           alt="{{ member.name }}" class="team-photo">
      {% endif %}
      <div class="team-body">
        <h4 class="team-name">{{ member.name }}</h4>
        {% if member.info %}<p class="team-role"><em>{{ member.info }}</em></p>{% endif %}
        {% if member.web %}<p><a href="{{ member.web }}" target="_blank">Home page</a></p>{% endif %}
        {% if member.number_educ %}
        <ul class="team-edu">
          {% for i in (1..member.number_educ) %}
            <li>{{ member['education' | append: i] }}</li>
          {% endfor %}
        </ul>
        {% endif %}
      </div>
    </div>
  </div>
{% endfor %}
</div>


### Master and Bachelor Students
<ul class="student-list">
{% for member in site.data.students %}
  <li>
    <strong>{{ member.name }}</strong>
    {% if member.info %} — {{ member.info }}{% endif %}
    {% if member.number_educ %}
      <ul>
        {% for i in (1..member.number_educ) %}
          <li>{{ member['education' | append: i] }}</li>
        {% endfor %}
      </ul>
    {% endif %}
  </li>
{% endfor %}
</ul>


### External Collaborators
<ul class="student-list">
{% for member in site.data.external_collaborators %}
  <li>
    <strong>{{ member.name }}</strong>
    {% if member.info %} — {{ member.info }}{% endif %}
  </li>
{% endfor %}
</ul>



### Alumni
<ul class="student-list">
{% for member in site.data.alumni_members %}
  <li>
    <strong>{{ member.name }}</strong>
    {% if member.info %} — {{ member.info }}{% endif %}
  </li>
{% endfor %}
</ul>