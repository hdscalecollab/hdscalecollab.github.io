---
layout: page
title: Project
title_headline_text: Projects of HDScaleCollab
permalink: /project/
---

## Active Projects

<div class="content list">
  {% for post in site.posts %}
    {% if post.categories contains 'project_active' %}
    <div class="list-item">
      <p class="list-post-title">
            <div class="row">
                <div class="col-sm-4">
                    <img src="{{site.baseurl}}/assets/img/post//{{ post.header-img }}">
                    <!-- <img src="/{% if post.header-img %}{{ post.header-img }}{% else %}{{ site.header-img }}{% endif %}"> -->
                </div>
                <div class="col-sm-8">
                    <a href="{{ post.url | prepend: site.baseurl }}">
                      <h3 class="post-title">
                        {{ post.title }}
                      </h3>
                    </a>
                    <p class="list-post-title">
                      posted on {{ post.date | date: "%B %-d, %Y" }}
                    </p>
                    <p class="list-detail" >
                      {{ post.content | strip_html | truncatewords:30 }}
                    </p>
                </div>
            </div>
            <hr/>
      </p>
    </div>
    {% endif %}
  {% endfor %}
</div>

## Past Projects
2020-2021: Genomic and Environmental Determinants of Infant Deaths in San Diego County in 2015-2022
- Goal: Understand genetic causes of infant mortality in 1,000 infant deaths in San Diego County and explore environmental contributors to those deaths to inform future prevention strategies.

2016-2019: Hispanic Access and Exposure to the Built Food Environment Funding: NSF, Geography and Spatial Sciences Program (BCS-1561112)
- Goal: Using sensor-based data collection methods, assess the exposure and access of Hispanics in the San Diego region to the built food environment.

2015-2017: Nucleotides to Neighborhoods: Obesity-Related Association Networks Spanning Genomes, Behaviors, and Built Environment Funding: UCSD Center for Computational Biology and Bioinformatics and San Diego Center for Systems Biology
- Goal: To assess as many levels of health related to obesity as possible including neighborhood, physical activity, and omics.
