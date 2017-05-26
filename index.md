---
layout: default
---

## Hi this is my site

This is the **index** page.

This site is built with Jekyll.

<img class="col one right" src="/assets/trap1d.jpeg">

<br/>
Write your biography here. Tell the world about yourself. Link to your favorite <a href="http://reddit.com" target="blank">subreddit</a>.

| I am text to the left  | ![trap1d](/assets/trap1d.jpeg){:height="50%" width="50%"} |
| I am text to the left  | ![trap1d](/assets/trap1d.jpeg){:class="img-responsive"} |


  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
        <span class="post-meta">{{ post.date | date: date_format }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
        </h2>
      </li>
    {% endfor %}
  </ul>
