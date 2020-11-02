---
layout: page
title: FAQs
menu: "FAQs"
order: 4
related:
  - title: "Learn More About Related Laws and Policies"
    url: "https://www.ucsc.edu/"
  - title: "Report Hate and Bias"
    url: "https://reporthate.ucsc.edu/"
---
<ul class="collapsible" data-collapsible="accordion">
  {% for faq in site.data.faqs %}
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

