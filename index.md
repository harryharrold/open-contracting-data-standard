---
layout: home
title: Welcome to the Open Contracting Data Standard Project
---
Strapline - up to ten words

Elevator pitch - up to 50 words

Call to action: to "Project" page

Current work - Call to action to read "Current work", and link to the most recent item on the "Progress" page

Join us - Call to action to read "Join us", and link to "Get involved" page


        <div>
            {% assign post = site.posts.first %}
            <a href="{{site.baseurl}}{{ post.url }}">
                <div>
                    <div>
                        {% if post.image %}
                        <img src="{{ post.image }}"/>
                        {% elsif post.snippet %}
                        <p>{{ post.snippet }}</p>
                        {% elsif post.content %}
                        <p>{{ post.content | strip_html | truncate: 130}}...</p>
                        {% else %}
                        <p>Read latest.</p>
                        {% endif %}
                    </div>
                    <div>
                        <button role="button">Read latest</button>
                    </div>
                </div>
            </a>
        </div>
