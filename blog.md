---
layout: default
title: Compliance Insights
permalink: /blog/
---

<section class="hero" style="padding-bottom: 100px;">
    <div class="container">
        <span style="color: var(--brand-red); font-weight: 700; text-transform: uppercase; letter-spacing: 1px; font-size: 0.9rem; display: block; margin-bottom: 10px;">
            Resource Centre
        </span>
        <h1>
            Latest <span style="color: var(--brand-navy);">Insights.</span>
        </h1>
        <p>
            Expert guidance on UK Fire Safety Regulations, BS 7671 changes, and property compliance standards.
        </p>
    </div>
</section>

<div class="container">
    <div class="card-grid">
        
        {% for post in site.posts %}
        <a href="{{ post.url | relative_url }}" class="service-card" style="display: block; text-decoration: none;">
            
            <span style="background: var(--bg-offset); color: var(--brand-navy); font-size: 0.8rem; font-weight: 700; padding: 6px 12px; border-radius: 4px; text-transform: uppercase; display: inline-block; margin-bottom: 20px;">
                {{ post.category }}
            </span>
            
            <h3 style="font-size: 1.3rem; margin-bottom: 15px; line-height: 1.3;">
                {{ post.title }}
            </h3>
            
            <p style="color: var(--text-muted); font-size: 0.95rem; margin-bottom: 25px;">
                {{ post.excerpt | strip_html | truncatewords: 20 }}
            </p>
            
            <div style="border-top: 1px solid var(--border-subtle); padding-top: 20px; color: var(--brand-red); font-weight: 700; font-size: 0.9rem; display: flex; align-items: center; justify-content: space-between;">
                Read Article
                <span>&rarr;</span>
            </div>
        </a>
        {% endfor %}

    </div>
</div>
