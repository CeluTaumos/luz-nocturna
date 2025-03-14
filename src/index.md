---
title: Luz Nocturna
layout: "main.njk"
---

<div class="ag-format-container">
    <div class="ag-courses_box">
        {% for post in collections.posts %}
        <div class="ag-courses_item">
            <a href="{{ post.url }}" class="ag-courses-item_link">
                <div class="ag-courses-item_bg"></div>

                <div class="ag-courses-item_title">
                    {{ post.data.title }}
                </div>

                {% if post.data.date %}
                <div class="ag-courses-item_date-box">
                    Publicado el:
                    <span class="ag-courses-item_date">
                        {{ post.data.date | date: "%d/%m/%Y" }}
                    </span>
                </div>
                {% endif %}
            </a>
        </div>
        {% endfor %}
    </div>
</div>
