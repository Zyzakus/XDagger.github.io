---
layout: xfsLayout
title: XDAG Funding System
---

Dagger (XDAG) is a community project with many contributors who use their spare time to contribute to the project. With the XDAG Funding System, proposals can be funded and more members can get involved in the community.

### Ideas Fundraising Work in Progress Completed Proposals
<div id="newsContainer">
<div id="title" class="flex-item">
{% for toplevel in site.data.xfs %}
    {% if toplevel.stage == "Ideas" %}
        {% for proposal in toplevel.proposals limit:2 %}
            <h3><a href="{{site.baseurl}}/{{proposal.url}}">{{proposal.name}}</a></h3>
            <p>Summary: {{proposal.summary}} 
            Author: {{proposal.author}}</p>
        {%endfor%}
    {%endif%}
{%endfor%}
<p><a href="{{ '/xdag-funding-system/proposals/' | relative_url }}">See all Ideas</a></p>
</div>

<div id="title" class="flex-item">
{% for toplevel in site.data.xfs %}
    {% if toplevel.stage == "Fundraising" %}
        {% for proposal in toplevel.proposals limit:2 %}
            <h3><a href="{{site.baseurl}}/{{proposal.url}}">{{proposal.name}}</a></h3>
            <p>Summary: {{proposal.summary}}</p>
            <p>Author: {{proposal.author}}</p>
        {%endfor%}
    {%endif%}
{%endfor%}
<p><a href="{{ '/xdag-funding-system/proposals/' | relative_url }}">See all Fundraising</a></p>
</div>

<div id="title" class="flex-item">
{% for toplevel in site.data.xfs %}
    {% if toplevel.stage == "Work in Progress" %}
        {% for proposal in toplevel.proposals limit:2 %}   
            <h3><a href="{{site.baseurl}}/{{proposal.url}}">{{proposal.name}}</a></h3>
            <p>Summary: {{proposal.summary}}</p>
            <p>Author: {{proposal.author}}</p>
        {%endfor%}
    {%endif%}
{%endfor%}
<p><a href="{{ '/xdag-funding-system/proposals/' | relative_url }}">See all Work in Progress</a></p>
</div>

<div id="title" class="flex-item">
{% for toplevel in site.data.xfs %}
    {% if toplevel.stage == "Completed Proposals" %}
        {% for proposal in toplevel.proposals limit:2 %}
            <h3><a href="{{site.baseurl}}/{{proposal.url}}">{{proposal.name}}</a></h3>
            <p>Summary: {{proposal.summary}}</p>
            <p>Author: {{proposal.author}}</p>
        {%endfor%}
    {%endif%}
{%endfor%}
<p><a href="{{ '/xdag-funding-system/proposals/' | relative_url }}">See all Completed Proposals</a></p>
</div>
</div>
You can also support the community by sending XDAG to the following address:

<p class="centerWallet">{{site.offical}}</p>