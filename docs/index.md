---
homepage: true
layout: product
title: Engineering Guidance and Standards
description: Build better applications by working to agreed Home Office engineering principles and standards.
# hide duplicate title in page title
options:
  header:
    productName: ''
---
<div class="govuk-grid-row">
{% for item in collections["homepage"] %}
  <section class="govuk-grid-column-one-third-from-desktop govuk-!-margin-bottom-8">
    <h2 class="govuk-heading-m govuk-!-font-size-27">{{ item.data.title }}</h2>
    <p class="govuk-body">{{ item.data.description | markdown("inline") }}</p>
    <p class="govuk-body"><a class="govuk-link govuk-!-font-weight-bold" href="{{ item.url | url }}">Learn about {{ item.data.title | lower }}</a></p>
  </section>
{% endfor %}
</div>