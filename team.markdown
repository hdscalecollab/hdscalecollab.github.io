---
layout: page
title: Team
title_headline_text: HDScale Collab Team
permalink: /team/
---

<header>
  <div class="row justify-content-center">
    <h2>{{ page.title_headline_text | escape }}</h2>
  </div>

</header>
<hr style="width:40%">


<!-- Staff -->

<h2><a id="staff"></a>Staff</h2>
{% assign members = site.data.team_members | where: 'category', 'staff' | sort: 'date' %}
{% for member in members %}
  <div class="card border-light mb-3">
      <div class="row mt-3">
          <div class="col-md-3 d-flex justify-content-center mx-auto my-auto">
            <a>
            <!-- <a href={{member.url}}> -->
                  <img src="{{ site.url }}{{ site.baseurl }}/assets/img/member_pics/{{ member.photo }}"
                      class="card-img rounded-circle img-responsive img-thumbnail"
                      style="max-width: 200px;"/>
              </a>
          </div>

          <div class="col-md-9">
              <div class="card-body">
              <h4 class="card-title">{{ member.name }}</h4>
              <h6 class="card-subtitle mb-2">{{  member.info }}</h6>
              <p class="card-text">{{ member.bio }}</p>
              </div>
          </div>
      </div>
  </div>
{% endfor %}

<br>

<!-- Members -->

<h2><a id="member"></a>Members</h2>
{% assign members = site.data.team_members | where: 'category', 'member' | sort: 'date' %}
{% for member in members %}
<div class="card border-light mb-3 team-member-card">
    <div class="row mt-3">
        <div class="col-md-3 d-flex justify-content-center mx-auto my-auto">
            <a>
            <!-- <a href={{member.url}}> -->
                <img src="{{ site.url }}{{ site.baseurl }}/assets/img/member_pics/{{ member.photo }}"
                    class="card-img rounded-circle img-responsive img-thumbnail"
                    style="max-width: 200px;"/>
            </a>
        </div>

        <div class="col-md-9">
            <div class="card-body">
            <h4 class="card-title">{{ member.name }}</h4>
            <h6 class="card-subtitle mb-2">{{  member.info }}</h6>
            <p class="card-text">{{ member.bio }}</p>
            </div>
        </div>
    </div>
</div>
{% endfor %}

<br>

<!-- Alumni -->

<h2><a id="alumni"></a>Alumni</h2>
<hr>
<div class="row">
{% assign members = site.data.team_members | where: 'category', 'alumni' | sort: 'date' | reverse %}
{% for member in members %}
   <div class="col-md-6 pb-4">
    <h5 class="mb-0 pb-0">{{ member.name }}</h5>
    <h7 class="card-subtitle">{{  member.info }}</h7>
   </div>
{% endfor %}
</div>
