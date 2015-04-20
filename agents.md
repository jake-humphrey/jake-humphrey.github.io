---
layout: page
title: Agents
permalink: /agents/
---

Our members are trained Equity Marketing Specialist (EMS). An EMS is a real estate agent who has achieved a high level of training in marketing, real estate counseling, real estate taxation, financing, real estate management and exchanges. The exchange process gives many owners the opportunity to diversify, preserve, and increase the wealth of their real estate investments. The exchange process brings more buyers to the market, creates additional opportunities and preserves wealth.

Please contact us when you are ready to discuss the opportunities that Exchanges and Equity Marketing present.

<ul class="agent-list">
{% for agent in site.categories.agents %}
	<li class="agent">
		<div class="agent-col-1 agent-image"></div>
		<div class="agent-col-2 agent-info">
			<a class="agent-name" href="{{ agent.url }}">{{ agent.title }}</a>
			<p class="agent-meta">{{ agent.position }} • <a href="mailto:{{ agent.email }}">Email</a></p>
			<p>{{ agent.excerpt }}</p>
		</div>
	</li>
{% endfor %}
</ul>