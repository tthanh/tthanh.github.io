---
layout: default
permalink: /
---
  <div class="profile-container">
    <img src="/assets/profile.jpg" alt="Profile Picture">
    <div style="border-bottom: ">
      <!-- <h5>Hi! I'm Thanh, a Full-Stack .NET Developer. 👨‍💻</h5> -->
      <p>Hi! I specialize in building high-performance web apps and am eager to join your team on next exciting projects.</p>
      <div class="socials">
        <a href="mailto:tranthuanthanh.dl@gmail.com" class="social-btn btn-email"><i class="fas fa-envelope"></i></a>
        <a target="_blank" href="https://www.linkedin.com/in/tranthuanthanh" class="social-btn btn-linkedin"><i class="fab fa-linkedin-in"></i></a>
        <a target="_blank" href="https://www.github.com/tthanh" class="social-btn btn-github"><i class="fab fa-github"></i></a>
        <a href="/projects" class="my-btn btn-projects"><i class="fas fa-pencil-ruler"></i>My Projects</a>
        <a href="/blog" class="my-btn btn-blog"><i class="fas fa-pen"></i>My Blog</a>
      </div>
    </div>
  </div>
<div class="row">
  <div class="col mt-4">
    <div class="skill-body timeline-body bg-themed">
      <div class="timeline-item">
          <div class="content">
            <div class="skills-container">
  <div class="skill bg-themed">
    <span>
      <b>Languages: </b>C#, Go, Python, Javascript, Typescript
    </span>
  </div>
  <div class="skill bg-themed">
    <span>
      <b>Database: </b> SQL Server, PostgreSQL, MongoDB, DynamoDB, Redis
    </span>
  </div>
  <div class="skill bg-themed">
    <span>
      <b>Frameworks: </b> .NET, Gin, React, Blazor, .NET MVC
    </span>
  </div>
  <div class="skill bg-themed">
    <span>
      <b>Cloud Services: </b> AWS, VMWare Private Cloud
    </span>
  </div>
  <div class="skill bg-themed">
    <span>
      <b>Architectures: </b>Microservices, DDD, Clean Architecture, Event-Driven Architecture.
    </span>
  </div>
  <div class="skill bg-themed">
    <span>
      <b>CI/CD: </b>AWS CodePipeline, Kubernetes, GitLab CI/CD, Bitbucket Pipelines
    </span>
  </div>
  <div class="skill bg-themed">
    <span>
      <b>Methodologies: </b>Agile
    </span>
  </div>
   <div class="skill bg-themed">
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
          <div class="content exp-content">
            <h3>{{ item.title }}</h3>
            <div class="timeline-date-loc">
              <h6 class="date">{{ item.from }} — {{ item.to }}</h6>
              <h6 class="date timeline-loc">{{ item.location }}</h6>
            </div>
            <div class="exp-content-skills">
            {% for skill in item.skills %}
                <span class="badge badge-primary">{{ skill }}</span>
              {% endfor %}
            </div>
            <p>
              {{ item.description }}
            </p>
          </div>
        </div>
      {% endfor %}
    </div>
  </div>
</div>
<div class="more-about">
  <h4 class="section-title">Feel free to take a look at:</h4>
  <div class="more-about-links">
  <a href="/projects" class="my-btn btn-projects"><i class="fas fa-pencil-ruler"></i>My Projects</a>
  <a href="/blog" class="my-btn btn-blog"><i class="fas fa-pen"></i>My Blog</a>
  </div>
</div>
