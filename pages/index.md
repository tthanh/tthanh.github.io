---
layout: default
permalink: /
---
  <div class="profile-container">
    <img src="/assets/profile.jpg" alt="Profile Picture">
    <div style="border-bottom: ">
      <h5>Hi! I'm Thanh, a Full Stack .NET Developer. 👨‍💻</h5>
      <br>
      <p>I specialize in building high-performance web apps and am eager to join your team to on next exciting projects.</p>
    </div>
  </div>
<!-- <h2 class="section-title">Skills</h2> -->
<div class="row">
  <div class="col mt-4">
    <div class="skill-body timeline-body bg-themed">
      <div class="timeline-item">
          <div class="content">
            <div class="skills-container">
  <div class="skill">
    <span>
      <b>Languages: </b>C#, Go, Python, Javascript, Typescript
    </span>
  </div>
  <div class="skill">
    <span>
      <b>Database: </b> SQL Server, PostgreSQL, MongoDB, DynamoDB, Redis
    </span>
  </div>
  <div class="skill">
    <span>
      <b>Frameworks: </b> .NET, Gin, React, Blazor, .NET MVC
    </span>
  </div>
  <div class="skill">
    <span>
      <b>Cloud Services: </b> AWS, VMWare Private Cloud
    </span>
  </div>
  <div class="skill">
    <span>
      <b>Architectures: </b>Microservices, DDD, Clean Architecture, Event-Driven Architecture.
    </span>
  </div>
  <div class="skill">
    <span>
      <b>CI/CD: </b>AWS CodePipeline, Kubernetes, GitLab CI/CD, Bitbucket Pipelines
    </span>
  </div>
  <div class="skill">
    <span>
      <b>Methodologies: </b>Agile
    </span>
  </div>
   <div class="skill">
    <span>
      <b>Other: </b>Docker, CloudFormation, ELK, SignalR, gRPC, GraphQL
    </span>
  </div>
</div>
          </div>
        </div>
    </div>
  </div>
</div>

<h2 class="section-title">Experience</h2>
<div class="row">
  <div class="col mt-4">
    <div class="timeline-body bg-themed">
      {% for item in site.data.timeline %}
        <div class="timeline-item">
          <div class="content">
            <h3>{{ item.title }}</h3>
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
<div class="more-about">
  <h4 class="section-title">Feel free to take a look at:</h4>
  <a href="/projects" class="btn">My Projects</a>
  <a href="/blog" class="btn">My Blog</a>
</div>
