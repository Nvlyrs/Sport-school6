---
layout: default
title: Методические материалы
---

<main class="main">
            <section class="info-section">
                <div class="info-section__content-wrapper content-wrapper">
                    <h2 class="info-section__title default-section-title">Методические материалы</h2>
                    <h3 class="info-section__card-title default-card-title">Нвигация по страцие</h3>
                    <ul class="info-section__navbar">
                        {% for item in site.data.matireals.sections %}
                        <li><a href="#{{item.anchor}}">{{item.id}}. {{item.header}}</a></li>
                        {% endfor %}
                    </ul>
                    {% for item in site.data.matireals.sections %}
                    <div class="info-section__document-block" id="{{item.anchor}}">
                        <h3 class="info-section__card-title default-card-title">{{item.id}}.{{item.header}}</h3>
                        <ul class="info-section__doc-list default-info-list">
                            {% for doc in item.matireals %}
                                {% if doc.date != "" %}
                                    <li> {{doc.date}} <br> <a href="{{doc.url}}">{{doc.title}}</a></li>
                                {% else %}
                                    <li><a href="{{doc.url}}">{{doc.title}}</a></li>
                                {% endif %}
                            {% endfor %}
                        </ul>
                    </div>
                    {% endfor %}
                </div>
            </section>
        </main>
