---
layout: category
title:  "Fashion"
top-word: "Explore"
image: "img/events/fa.jpg"
date:   2015-04-21 12:12:12
---
<section class="no-padding" id="portfolio">
    <div class="container-fluid">
        <div class="row no-gutter">
            {% for fashion in site.fashion %}
                <div class="col-lg-4 col-sm-6">
                    <a href="{{ fashion.url }}" class="portfolio-box">
                        <img src="{{ fashion.image }}" class="img-responsive" alt="fashion Image">
                        <div class="portfolio-box-caption">
                            <div class="portfolio-box-caption-content">
                                <div class="project-category text-faded">
                                    {{ fashion.subtitle }}
                                </div>
                                <div class="project-name">
                                    {{ fashion.title }}
                                </div>
                            </div>
                        </div>
                    </a>
                </div>
            {% endfor %}
        </div>
    </div>
</section>