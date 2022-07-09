---
title: Phase 1 Front End
url: 'this-is-a-url/ok'
---

{% assign topics = site.data.topics_by_date | where: 'phase', '1' | reverse %}


{% for topic in topics %}
  {{ topic.date | date: "%B %-d" }}
  : [{{ topic.title }}]({% link {{topic.url}} %})
    : [Lab]({{ topic.lab_url }}){: .label .label-mmntm-purple } [Resources]({{ topic.resources_url }}){: .label .label-mmntm-red }
{% endfor %}
