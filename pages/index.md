---
layout: default
permalink: /
---
<br><br>
Hello! My name is [Your Name], and I am a dedicated software developer based in Vietnam with 5 years of experience in the industry.

<div class="row">
{% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
{% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>


Want to find more about me? Check out my

<a href = "/projects">Projects</a>
<a href = "/blog">Blog</a>

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