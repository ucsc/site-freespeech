---
layout: page
title: FAQs
menu: "FAQs"
order: 4
---
<ul class="collapsible" data-collapsible="expandable">
  {% for faq in site.data.faqs %}
  <li class="faqs-list">
     <div class="collapsible-header"><i class="mdi-navigation-chevron-right"></i><div class="faq-title">{{ faq.question }}</div></div>
     <div class="collapsible-body">{{ faq.answer}}</div>
  </li>
  {% endfor %}
</ul>

{% include collapsible.html %}
