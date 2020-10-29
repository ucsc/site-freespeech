---
layout: page
title: FAQs
menu: "FAQs"
order: 4
---
<ul class="collapsible" data-collapsible="accordion">
  {% for faq in site.data.faqs %}
  <li class="faqs-list">
     <div class="collapsible-header">
      <div class="expand-icon"><i class="material-icons right more" aria-expanded="true">expand_more</i>
            <i class="material-icons right less" style="display: none" aria-expanded="false">expand_less</i></div>
      <div class="faq-title">{{ faq.question }}</div>
     </div>
     <div class="collapsible-body">{{ faq.answer}}</div>
  </li>
  {% endfor %}
</ul>

{% include collapsible.html %}
