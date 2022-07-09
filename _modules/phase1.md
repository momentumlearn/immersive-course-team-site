---
title: Phase 1 Front End
phase: 1
---

{% assign topics = site.data.phase1_topics | reverse %}


{% for topic in topics %}
  {{ topic.date | date: "%B %-d" }}
  : [{{ topic.title }}]({% link {{topic.url}} %})
    : [Lab]({{ topic.lab_url }}){: .label .label-mmntm-purple } [Resources]({% link {{ topic.resources_url }} %}){: .label .label-mmntm-red }
{% endfor %}
