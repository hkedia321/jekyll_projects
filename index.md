---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: default
---

<div class="container-fluid">
  <div class="landing-bg">
    <div class="overlay">
    </div>
    <div class="content">
      <div class="center">
        <img src="img/logo_white.png" class="responsive-img landing-logo" />
      </div>
      <div class="center">
        <h2 class="center white-text">Projects</h2>
        <div class="underline">

        </div>
      </div>
      <br /><br />
      <h5 class="center white-text">All the awesome work we have done!</h5>
    </div>
  </div>
</div>
<div class="projects-div-wrap">
<div class="container projects-container">
  <br />
  <div class="row">
    {% for post in site.posts %}
    <div class="col s12 m4">
      <div class="card hoverable project-card">
        <div class="date">
          <i class="fa fa-calendar" aria-hidden="true"></i> {{post.date | date: "%Y-%m-%d"}}
        </div>
        <div class="users">
          <i class="fa fa-users" aria-hidden="true"></i> {{post.users}} users
        </div>
        <h4 class="center project-title">{{post.title}}</h4>
        <p class="left-align project-desc">
          {{post.description}}
        </p>
        <div class="see-div ver-align-middle" title="view project">
        <a href="" class="see-a ver-align-middle">
      <i class="fa fa-eye fa-2x ver-align-middle" aria-hidden="true"></i>
        </a>
      </div>
        <div class="more-div" title="read more">
        <a href="{{post.url}}" class="btn waves-effect read-btn ver-align-middle">
          Read More <i class="fa fa-arrow-right fa-2x ver-align-middle white-text" aria-hidden="true"></i>
        </a>
      </div>
      </div>
    </div>
      {% endfor %}
  </div>
</div>
</div>
<div class="container">
  <footer class="center">
    <img src="{{site.url}}/img/logo_black.png" class="footer-logo" />
    <div >
    <a href="" target="_blank"><i class="fa fa-github" aria-hidden="true"></i></a>
    <a href="" target="_blank"><i class="fa fa-twitter" aria-hidden="true"></i></a>
    <a href="" target="_blank"><i class="fa fa-facebook" aria-hidden="true"></i></a>
    <a href="" target="_blank"><i class="fa fa-rss" aria-hidden="true"></i></a>
  </div>
  <div>
    &copy; 2017 Google Developers
  </div>
  </footer>
</div>
