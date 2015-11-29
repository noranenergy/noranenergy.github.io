---

layout: default
title: Team
subtitle: Our team of directors

team: 
  - name: 'Adrian Hall'
    page: adrian.html
    image: adrian.png
    title: 'Managing Director'

  - name: 'Grant Knight'
    page: grant.html
    image: grant.png
    title: 'Business Development Director'


  - name: 'Nader Behjat'
    page: nader.html
    image: nader.png
    title: 'Technical Director - Drilling & Completions'


  - name: 'Clive Bjøru-Swatton'
    page: clive.html
    image: clive.png
    title: 'Operations Director'

  - name: 'Charles Evans'
    page: charles.html
    image: charles.png
    title: 'Technical Director - Subsurface'
    
  - name: 'Dr. Mohammad Hajiarab'
    page: mohammad.html
    image: mohammad.png
    title: 'Technical Director - Facilities'
    
  
---

<ul class="team_members">
{% for member in page.team %}
  <li>
    <a href="/team/{{ member.page }}">

      <div style="display: block;">
        <img src="/images/{{member.image}}" alt="{{member.name}}" />
      </div>
      <div style="display: inline-block;">
        <span class="name">{{ member.name }}</span>
        <span class="title">{{ member.title }}</span>
      </div>
    </a>
  </li>
{% endfor %}
</ul>
