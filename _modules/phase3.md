---
title: Phase 3
phase: 2
---

{% assign topics = site.data.phase3_topics | reverse %}


{% for topic in topics %}
  {{ topic.date | date: "%B %-d" }}
  : **{{topic.tag}}**{: .label .{{topic.tag}}-label } [{{ topic.title }}]({% link {{topic.url}} %})
    : [Lab]({{ topic.lab_url }}){: .label .lab-label } [Resources]({% link {{ topic.resources_url }} %}){: .label .resources-label }
{% endfor %}

