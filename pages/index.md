---
layout: default
permalink: /
---
<!-- <br> -->
  <div class="profile-container">
    <img src="/assets/profile.jpg" alt="Profile Picture">
    <div>
      <h5>Hi! I'm Thanh, a Full Stack .NET Developer. 👨‍💻</h5>
      <br>
      <p>I specialize in building high-performance web apps and am eager to join your team to work on exciting projects.</p>
    </div>
  </div>
<br><br>
<!-- <h2>Skills</h2> -->
<h2>Skills</h2>
<div class="row">
<!-- {% include about/skills.html title="Programming Skills" source=site.data.programming-skills %} -->
<!-- {% include about/skills.html title="Other Skills" source=site.data.other-skills %} -->
</div>

<br><br>
<h2>Experience</h2>
<div class="row">
<!-- {% include about/timeline.html %} -->
<div class="col mt-4">
  <div class="timeline-body bg-themed">
    {% for item in site.data.timeline %}
      <div class="timeline-item">
        <div class="content">
          <h2>{{ item.title }}</h2>
          <div class="timeline-date-loc">
            <h6 class="date">{{ item.from }} — {{ item.to }}</h6>
            <h6 class="date timeline-loc">{{ item.location }}</h6>
          </div>
          <p>{{ item.description }}</p>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
</div>
<br><br>
<h2>More about me</h2>

Take a look at:

<a href = "/projects">My Projects</a>
<a href = "/blog">My Blog</a>

Or reach out to me through


<div class="container-fluid justify-content-center">

  {%- assign unfocused_color = "6c757d" -%}

  {% for account in site.author %}

    {%- assign service_name = account[0] -%}
    {%- assign service_data = site.data.social-media[service_name] -%}
    {%- if service_data -%}    
    <a class="social mx-1"  href="{{ service_data.url }}{{ account[1] }}"
       style="color: #{{ unfocused_color }}"
       onMouseOver="this.style.color='#{{ service_data.color }}'"
       onMouseOut="this.style.color='#{{ unfocused_color }}'">
      <i class="{{ service_data.icon }} fa-1x"></i>
    </a>
    {%- endif -%}
  
  {% endfor %}

</div>