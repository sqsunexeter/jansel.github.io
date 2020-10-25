---
layout: page
permalink: /publications/index.html
title: Publications
pubs: 
  - author: "R. Liu, M. Xie and S. Sun"
    title: "Reconstructing Positive Surveys from Negative Surveys by Improved Artificial Immune Network"
    month: "June"
    year: "2018"
    booktitle: "IEEE Symposium Series on Computational Intelligence (SSCI)"
    url: "https://ieeexplore.ieee.org/abstract/document/8628929"
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    
    

---

# Publications

{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

<!--
# Patents
See [Google Patent Search results](https://patents.google.com/?inventor=Jason+Ansel,-Lango&num=100&sort=old).
-->
