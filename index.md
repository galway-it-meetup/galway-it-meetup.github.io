---
layout: index
---

<div class="wrapper">
    <div class="inner">
    <!-- Banner -->
    <section id="banner">
    <div class="items">
        <section class="accent2">
        <h1>Past Events</h1>
        {%- assign _past_events = site.posts | where: 'categories', 'past_events' -%}
        {%- assign _most_recent = _past_events.first -%}

        <a href="{{_most_recent.url}}"> 
            <b>
                {{_most_recent.date  | date: "%B %d, %Y" }}
            </b> : 
            <b>
                {{_most_recent.title}}
            </b>
        </a>
        <br/>
        <br/>
        <ul class="actions special">
            <li>
            <a
                href="/past_events"
                class="button primary"
                >More</a>
            </li>
        </ul>
        </section>
        <section class="accent3">
        <h1>Upcoming Events</h1>
        {%- assign _upcoming_events = site.posts | where: 'categories', 'upcoming_events' -%}
        {%- assign _soonest = _upcoming_events.first -%}
        
        {% if _soonest%}
            
            {% for post in site.posts %}
            {% if post.tags contains 'upcoming-events' %}

                <a href="{{post.url}}">
                    <b>
                        {{post.date  | date: "%B %d, %Y" }} : 
                    </b>
                    <b>
                        {{post.title}}
                    </b>
                </a>
                <br/>    
                <br/>
            {% endif %}
            {% endfor %}
            
            <br/> 
            <ul class="actions special">
                <li>
                <a
                    href="/upcoming_events"
                    class="button primary"
                    >More</a
                >
                </li>
            </ul>
        {% else %}
            <ul class="actions special">
                <li>
                <a
                    href="https://www.eventbrite.ie/o/galway-it-115249290071"
                    class="button primary"
                    >Eventbrite</a
                >
                </li>
                <li>
                <a
                    href="https://www.meetup.com/galway-information-technology/events/"
                    class="button primary"
                    >Meetup</a
                >
                </li>
            </ul>
        {% endif %}
        </section>
    </div>
    <div class="slider">
        <article>
        <img
            src="/images/pic01.jpg"
            alt=""
            data-position="bottom right"
        />
        </article>
        <article>
        <img
            src="/assets/1.4/photos/10.jpeg"
            alt=""
            data-position="bottom right"
        />
        </article>
        <article>
        <img
            src="/images/pic02.jpg"
            alt=""
            data-position="bottom right"
        />
        </article>
        <article>
        <img
            src="/assets/1.7/photos/4.jpg"
            alt=""
            data-position="bottom right"
        />
        </article>
        <article>
        <img src="/images/pic03.jpg" alt="" data-position="top left" />
        </article>
        <article>
        <img
            src="/assets/2.1/photos/4.jpg"
            alt=""
            data-position="bottom right"
        />
        </article>
    </div>
    </section>
</div>
</div>

<!-- Wrapper -->
<div class="wrapper">
<div class="inner">
    <!-- Section -->
    <section class="main">
    <header class="major">
        <h2>Welcome to Galway IT Meetup</h2>
        <p>
        We are a community based in the PorterShed in Galway, Ireland.
        We meet monthly in Galway to discuss and learn about different
        topics of interest to those who work in tech or who just love
        it!
        </p>
    </header>
    <div class="features">
        <section>
        <span
            class="icon solid fa-map-location-dot major accent2"
        ></span>
        <h3>Where?</h3>
        <p>
            We're usually hosted by the
            <a href="https://portershed.com/market-street/">PorterShed</a>
            on Market Street in Galway. If you need directions, you can
            find them
            <a href="https://maps.app.goo.gl/vyqddN1QLvtxyzRx9">here</a>.
        </p>
        </section>
        <section>
        <span class="icon solid fa-envelope major accent4"></span>
        <h3>What?</h3>
        <p>
            We've covered a huge range of topics, from AI developments to
            Galway's surprising history with technology. We're always
            looking for new speakers and topics, so if you have an idea,
            please reach out!
        </p>
        </section>
        <section>
        <span
            class="icon solid fa-solid fa-calendar-days major accent3"
        ></span>
        <h3>When?</h3>
        <p>
            Our dates shift from month to month to faciltate our speakers.
            Follow us on
            <a href="https://www.instagram.com/galway.it.meetup/"
            >Instagram</a
            >
            or
            <a href="https://www.meetup.com/galway-information-technology"
            >Meetup</a
            >
            to stay up to date with the next events.
        </p>
        </section>
    </div>
    </section>
</div>
</div>
<div class="wrapper">
<div class="inner">
    <!-- Section -->
    <section class="main accent5">
    <header class="major">
        <h2>Sponsors</h2>
        <p>
        While we have sponsors who help out with individual events, we also have some annual sponsors who support us and deserve a special shout-out:
        </p>
    </header>
    <ul class="actions fit" id="sponsors">
        <li>
        <a href="https://portershed.com/" target="_blank">
            <img src="/assets/sponsors/portershed.svg" height="70"/>
        </a>
        </li>
        <li>
        <a href="https://www.marteye.ie/" target="_blank">
            <img src="/assets/sponsors/marteye.svg" height="70"/>
        </a>
        </li>
    </ul>
    </section>
</div>
</div>
<div class="wrapper">
<div class="inner">
    <!-- Section -->
    <section class="main accent3">
    <header class="major">
        <h2>Community Survey</h2>
        <p>
        We're always looking for feedback and ideas on events, talks and
        workshops to run! Click the link below to access a survey where
        you can pass us along your feedback.
        </p>
        <p>
        Want to talk about what your learned building your latest
        project? Or maybe you have an idea for a workshop you'd like to
        run? We'd love to hear from you! Fill out the survey or contact
        us directly for a chat!
        </p>
    </header>
    <ul class="actions fit">
        <li>
        <a
            href="https://forms.gle/FXhGsr7U3yEpZkMR9"
            class="button primary fit"
            >Feedback Survey</a
        >
        </li>
    </ul>
    </section>
</div>
</div>