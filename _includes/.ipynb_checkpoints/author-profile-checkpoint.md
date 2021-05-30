{% include base_path %}

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

<div itemscope itemtype="http://schema.org/Person">

  <div class="author__avatar">
    {% if author.avatar contains "://" %}
    	<img src="{{ author.avatar }}" alt="{{ author.name }}">
    {% else %}
    	<img src="{{ author.avatar | prepend: "/images/" | prepend: base_path }}" class="author__avatar" alt="{{ author.name }}">
    {% endif %}
  </div>

  <div class="author__content">
    <h3 class="author__name">{{ author.name }}</h3>
    {% if author.bio %}<p class="author__bio">{{ author.bio }}</p>{% endif %}
  </div>

  <div class="author__urls-wrapper">
    <button class="btn btn--inverse">Follow</button>
    <ul class="author__urls social-icons">
      {% if author.location %}
        <li><i class="fa fa-fw fa-map-marker" aria-hidden="true"></i> {{ author.location }}</li>
      {% endif %}
      {% if author.employer %}
        <li><i class="fa fa-fw fa-map-marker" aria-hidden="true"></i> {{ author.employer }}</li>
      {% endif %}
      {% if author.email %}
        <li><a href="mailto:{{ author.email }}"><i class="fas fa-fw fa-envelope" aria-hidden="true"></i> {{ site.data.ui-text[site.locale].email_label | default: "Email" }}</a></li>
      {% endif %}
      {% if author.keybase %}
        <li><a href="https://keybase.io/{{ author.keybase }}"><i class="fas fa-fw fa-key" aria-hidden="true"></i> Keybase</a></li>
      {% endif %}
       {% if author.researchgate %}
        <li><a href="https://www.researchgate.net/profile/Sophie_Jentzsch{{ author.researchgate }}"><i class="fab fa-fw fa-researchgate" aria-hidden="true"></i> ResearchGate</a></li>
      {% endif %}
      {% if author.twitter %}
        <li><a href="https://twitter.com/sciphie{{ author.twitter }}"><i class="fab fa-fw fa-twitter-square" aria-hidden="true"></i> Twitter</a></li>
      {% endif %}
      {% if author.linkedin %}
        <li><a href="https://www.linkedin.com/in/sophie-jentzsch/{{ author.linkedin }}"><i class="fab fa-fw fa-linkedin" aria-hidden="true"></i> LinkedIn</a></li>
      {% endif %}
      {% if author.xing %}
        <li><a href="https://www.xing.com/profile/Sophie_Jentzsch/cv{{ author.xing }}"><i class="fab fa-fw fa-xing-square" aria-hidden="true"></i> XING</a></li>
      {% endif %}
      {% if author.github %}
        <li><a href="https://github.com/sciphie{{ author.github }}"><i class="fab fa-fw fa-github" aria-hidden="true"></i> Github</a></li>
      {% endif %}
      {% if author.stackoverflow %}
        <li><a href="https://www.stackoverflow.com/users/{{ author.stackoverflow }}"><i class="fab fa-fw fa-stack-overflow" aria-hidden="true"></i> Stackoverflow</a></li>
      {% endif %}
      {% if author.lastfm %}
        <li><a href="https://lastfm.com/user/{{ author.lastfm }}"><i class="fab fa-fw fa-lastfm-square" aria-hidden="true"></i> Last.fm</a></li>
      {% endif %}
      {% if author.steam %}
        <li><a href="https://steamcommunity.com/id/{{ author.steam }}"><i class="fab fa-fw fa-steam-square" aria-hidden="true"></i> Steam</a></li>
      {% endif %}
      {% if author.googlescholar %}
        <li><a href="{{ author.googlescholar }}"><i class="fas fa-fw fa-graduation-cap"></i> Google Scholar</a></li>
      {% endif %}
      {% if author.pubmed %}
        <li><a href="{{ author.pubmed }}"><i class="ai ai-pubmed-square ai-fw"></i> PubMed</a></li>
      {% endif %}
      {% if author.orcid %}
        <li><a href="https://orcid.org/0000-0001-6217-8814{{ author.orcid }}"><i class="ai ai-orcid-square ai-fw"></i> ORCID</a></li>
      {% endif %}
      {% if author.wikipedia %}
        <li><a href="https://en.wikipedia.org/wiki/User:{{ author.wikipedia }}"><i class="fab fa-fw fa-wikipedia-w" aria-hidden="true"></i> Wikipedia</a></li>
{% endif %}
    </ul>
  </div>
</div>
