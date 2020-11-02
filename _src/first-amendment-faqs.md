---
layout: page
title: First Amendment FAQs
permalink: /learn/first-amendment-faqs.html
left_navigation: learn
related:
  - title: "Learn More About Related Laws and Policies"
    url: "https://freespeech.ucsc.edu/learn/laws-policies.html"
  - title: "Report Hate and Bias"
    url: "https://reporthate.ucsc.edu/"
---

Generally, the First Amendment to the U.S. Constitution protects all speech, although the following forms of speech enjoy varying degrees of lesser protection:

<ul class="collapsible" data-collapsible="accordion">
  {% for faq in site.data.first-amendment-faqs %}
  <li class="faqs-list">
     <div class="collapsible-header">
      <div class="expand-icon">
        <i class="material-icons right more" aria-expanded="false" aria-controls="accordion-panel-{{ faq.content-marking }}">expand_more</i>
        <i class="material-icons right less" style="display: none" aria-expanded="true" aria-controls="accordion-panel-{{ faq.content-marking }}">expand_less</i>
      </div>
      <div class="faq-title">{{ faq.question }}</div>
     </div>
     <div class="collapsible-body" aria-labelledby="accordion-header-{{ faq.content-marking }}">{{ faq.answer }}</div>
  </li>
  {% endfor %}
</ul>