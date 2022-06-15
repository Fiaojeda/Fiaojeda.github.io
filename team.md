---
title: Learning by Teaching
layout: teams
description: Team
permalink: "/learning-by-teaching/"
intro_image_absolute: true
intro_image_hide_on_mobile: false
---


# Comparative Politics <br>

<img src='/images/world.png' width=600 aligned=right>


## What are political systems? <br>

A political system is a set of structures and agencies in charge of formulating and implementing the collective objectives of a society, or a group within society. 


## Why is it important to compare political systems? <br>

It is important to compare political systems to get to know more profoundly how certain countries work. It can also help shape the perception of reality and how power and decision making is done within national or international boundaries. 

To get the most out of this website, I encourage you to read some basic [definitions](/learning-by-teaching/definitions/) that will help you to understand how several political systems function around the world!

<div>
    <div class="row pt-6 pb-6">
        {% assign teams = site.team | where: "promoted", empty | sort: "weight" %}
        {% for team in teams %}
        <div class="col-12 col-md-4 mb-3">
            <div class="team team-summary">
                {% if team.image %}
                <div class="team-image">
                    <img width="60" height="60" alt="{{ team.title }}" class="img-fluid mb-2" src="{{ team.image | relative_url }}" />
                </div>
                {% endif %}
                <div class="team-meta">
                    <h2 class="team-name"><a href="{{ team.url | relative_url }}">{{ team.title }}</a></h2>
                    <p class="team-description">{{ team.jobtitle }}</p>
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</div>