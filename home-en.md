---
layout: default
permalink: /en/
---
<div class="container-fluid">
    <nav class="py-2">
        <div class="d-flex flex-wrap">
            <ul class="nav me-auto">
                <li class="nav-item">
                    <a class="nav-link active" href="https://ikovylyaev.com" style="padding-left: 0px!important">design</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link disabled" href="https://blog.ikovylyaev.com">blog</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="https://video.ikovylyaev.com">video</a>
                </li>
            </ul>
            <ul class="nav nav-2">
                <li class="nav-item">
                    <a class="nav-link" href="mailto:hi@ikovylyaev.com">hi@ikovylyaev.com</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="https://behance.net/ikovylyaev">behance</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="https://vk.com/ikovylyaev">vk</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="https://instagram.com/ikovylyaev">instagram</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="https://www.youtube.com/channel/UCf9GOVc0qKKPB-Ee3LfH_uw" style='padding-right: 0;'>youtube</a>
                </li>
            </ul>
            <ul class="nav nav-lang-1">
                <li class="nav-item">
                    <a class="nav-link" href="{{site.url}}">ru</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="{{site.url}}/en">en</a>
                </li>
            </ul>
        </div>
    </nav>
    <header class="py-3 mb-4">
        <div class="row">
            <a href="{{site.url}}" class="col-md-6 col-12">
                <img src="{{site.url}}/img/logo.svg" class="logotype" alt="ikovylyaev-logo">
            </a>
            <div class="col-md-6 col-12 text-right" style="position: relative">
                <ul class="nav nav-lang-2" style='position: absolute; right: 0;'>
                    <li class="nav-item">
                        <a class="nav-link" href="{{site.url}}">ru</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="{{site.url}}/en">en</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
        <div class="row">
            {% for post in site.design limit: 1 %}
            <div class='col'>
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
        <div class='row'>
            {% for post in site.design limit: 1 offset: 1 %}
            <div class="col-md-6 col-12">
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
            <div class='col-md-6 col-12'>
                {% for post in site.design limit: 2 offset: 2 %}
                    <div class='header-half'>
                        <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                        <div class='text'>
                            <h2 class="h3">{{ post.title }}</h2>
                            <span>{{ post.categories }}</span>
                            {% if post.concept == 'concept' %}
                                <span>concept</span>
                            {% endif %}
                            {% if post.link != "" %}
                                <a href='{{post.link}}' target="_blank">behance</a>
                            {% endif %}
                            {% if post.web != "" %}
                                <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                            {% endif %}
                        </div>
                    </div>
                {% endfor %}
            </div>
        </div>
        <div class='row'>
            <div class='col-md-6 col-12'>
                {% for post in site.design limit: 2 offset: 4 %}
                    <div class='header-half'>
                        <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                        <div class='text'>
                            <h2 class="h3">{{ post.title }}</h2>
                            <span>{{ post.categories }}</span>
                            {% if post.concept == 'concept' %}
                                <span>concept</span>
                            {% endif %}
                            {% if post.link != "" %}
                                <a href='{{post.link}}' target="_blank">behance</a>
                            {% endif %}
                            {% if post.web != "" %}
                                <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                            {% endif %}
                        </div>
                    </div>
                {% endfor %}
            </div>
            {% for post in site.design limit: 1 offset: 6 %}
            <div class="col-md-6 col-12">
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
        <div class='row'>
            {% for post in site.design limit: 1 offset: 7 %}
            <div class="col-md-6 col-12">
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
            <div class='col-md-6 col-12'>
                {% for post in site.design limit: 2 offset: 8 %}
                    <div class='header-half'>
                        <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                        <div class='text'>
                            <h2 class="h3">{{ post.title }}</h2>
                            <span>{{ post.categories }}</span>
                            {% if post.concept == 'concept' %}
                                <span>concept</span>
                            {% endif %}
                            {% if post.link != "" %}
                                <a href='{{post.link}}' target="_blank">behance</a>
                            {% endif %}
                            {% if post.web != "" %}
                                <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                            {% endif %}
                        </div>
                    </div>
                {% endfor %}
            </div>
        </div>
        <div class='row'>
            <div class='col-md-6 col-12'>
                {% for post in site.design limit: 2 offset: 10 %}
                    <div class='header-half'>
                        <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                        <div class='text'>
                            <h2 class="h3">{{ post.title }}</h2>
                            <span>{{ post.categories }}</span>
                            {% if post.concept == 'concept' %}
                                <span>concept</span>
                            {% endif %}
                            {% if post.link != "" %}
                                <a href='{{post.link}}' target="_blank">behance</a>
                            {% endif %}
                            {% if post.web != "" %}
                                <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                            {% endif %}
                        </div>
                    </div>
                {% endfor %}
            </div>
            {% for post in site.design limit: 1 offset: 12 %}
            <div class="col-md-6 col-12">
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
        <div class='row'>
            {% for post in site.design limit: 1 offset: 14 %}
            <div class="col-md-6 col-12">
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
            <div class='col-md-6 col-12'>
                {% for post in site.design limit: 2 offset: 15 %}
                    <div class='header-half'>
                        <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                        <div class='text'>
                            <h2 class="h3">{{ post.title }}</h2>
                            <span>{{ post.categories }}</span>
                            {% if post.concept == 'concept' %}
                                <span>concept</span>
                            {% endif %}
                            {% if post.link != "" %}
                                <a href='{{post.link}}' target="_blank">behance</a>
                            {% endif %}
                            {% if post.web != "" %}
                                <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                            {% endif %}
                        </div>
                    </div>
                {% endfor %}
            </div>
        </div>
        <div class='row'>
            <div class='col-md-6 col-12'>
                {% for post in site.design limit: 2 offset: 17 %}
                    <div class='header-half'>
                        <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                        <div class='text'>
                            <h2 class="h3">{{ post.title }}</h2>
                            <span>{{ post.categories }}</span>
                            {% if post.concept == 'concept' %}
                                <span>concept</span>
                            {% endif %}
                            {% if post.link != "" %}
                                <a href='{{post.link}}' target="_blank">behance</a>
                            {% endif %}
                            {% if post.web != "" %}
                                <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                            {% endif %}
                        </div>
                    </div>
                {% endfor %}
            </div>
            {% for post in site.design limit: 1 offset: 19 %}
            <div class="col-md-6 col-12">
                <div class='header'>
                    <div class='bg' style='background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;'></div>
                    <div class='text'>
                        <h2 class="h3">{{ post.title }}</h2>
                        <span>{{ post.categories }}</span>
                        {% if post.concept == 'concept' %}
                            <span>concept</span>
                        {% endif %}
                        {% if post.link != "" %}
                            <a href='{{post.link}}' target="_blank">behance</a>
                        {% endif %}
                        {% if post.web != "" %}
                            <p style='opacity: .6; display: inline;'>/</p>   <a href="https://{{post.web}}" target="_blank">{{post.web}}</a>
                        {% endif %}
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
            <footer class="d-flex flex-wrap justify-content-between align-items-center py-3 my-4 border-top">
                <div class="col-md-4">
                    <a href="{{site.url}}">
                        <img src="{{site.url}}/img/logo.svg" class="logotype-footer" alt="ikovylyaev-logo">
                    </a><br>
                    <a href="{{ site.url }}/privacy/" class='link' style="margin-right: 25px">privacy policy (ru)</a><br>
                    <a href="{{ site.url }}/terms/" class='link' style="margin-right: 25px">terms of use (ru)</a>
                </div>
                <ul class="nav col-md-4 justify-content-end list-unstyled d-flex nav-lang-2" style='margin-right: -1rem;'>
                    <li class="nav-item">
                        <a class="nav-link" href="mailto:hi@ikovylyaev.com">hi@ikovylyaev.com</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="https://behance.net/ikovylyaev">behance</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="https://vk.com/ikovylyaev">vk</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="https://instagram.com/ikovylyaev">instagram</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="https://www.youtube.com/channel/UCf9GOVc0qKKPB-Ee3LfH_uw" >youtube</a>
                    </li>
                </ul>
            </footer>
    
</div>