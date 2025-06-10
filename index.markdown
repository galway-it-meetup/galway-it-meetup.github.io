---

layout: home
title: Galway Information Technology Meetup Group
---

<br/>
<br/>
![Galway City: The Long Walk](/assets/home.png)
<p style="float:right;">Photo by <a href="https://unsplash.com/@mch1565?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash" target="_blank">Chan Hyuk Moon</a> on <a href="https://unsplash.com/photos/white-and-brown-concrete-building-beside-body-of-water-during-daytime-B0eewq7EbVY?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash" target="_blank">Unsplash</a></p>

<br/>
<br/>
<br/>

## Welcome to the Galway IT Meetup Group.

We are a community based in the [PorterShed](https://portershed.com/) in Galway, Ireland. We meet monthly in Galway to discuss and learn about software development, cyber security, game development, networking etc. 

<br/>
### Goal

We endeavour to meet once a month in Galway to learn, share, network and socialize. Galway has a vibrant and diverse community of tech students, workers, enthusiasts and companies. This group's goal is to provide a place for anyone interested in IT (software, hardware, development, research etc.) to come together and share ideas.

<br/>
### Plan

We will host and organise any event which our members are interested in. See the list of past events below for some examples, but feel free to suggest something completely different. For 2025 we'd like to branch out into computer hardware and 3D Printing.

<br/>
### Survey

To better cater towards our community, please fill out this [survey](https://forms.gle/FXhGsr7U3yEpZkMR9) if you have attended or are planning to attend any of our meetups.

<br/>
If you'd like to join us, you can join our: 
- [Meetup Group](https://www.meetup.com/galway-information-technology)
- [LinkedIn Group](https://www.linkedin.com/groups/14314350/)
- [Discord Server](https://discord.gg/6BV8A8DHbB)

If you want to speak / suggest a topic / get involved, please reach out on the above platforms or contact [Liam](https://www.linkedin.com/in/liamkrewer/) directly.

<br/>


{% if site.categories.upcoming_events and site.categories.upcoming_events.size != 0 %}
## Upcoming Events
<ul class="post-list">
{% for post in site.categories.upcoming_events %}
{% if post.url %}
<li>
    <span class="post-meta">{{post.date | date: "%A %-d %B %Y @ %H:%M"}}</span>
    <h3>
        <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
    </h3>
</li>
{% endif %}
{% endfor %}
</ul>
<br/>
{% endif %}

## Past Events

<ul class="post-list">
{% for post in site.categories.past_events %}
{% if post.url %}
<li>
    <span class="post-meta">{{post.date | date: "%A %-d %B %Y @ %H:%M"}}</span>
    <h3>
        <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
    </h3>
</li>
{% endif %}
{% endfor %}
</ul>
<br/>