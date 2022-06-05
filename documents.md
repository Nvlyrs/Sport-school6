---
layout: default
title: Документы
---
<main class="main">
            <section class="info-section">
                <div class="info-section__content-wrapper content-wrapper">
                    <h2 class="info-section__title default-section-title">Документы</h2>
                    {% for item in site.data.documents.sections %}
                    <div class="info-section__document-block">
                        <h3 class="info-section__card-title default-card-title">{{item.header}}</h3>
                        <ul class="info-section__doc-list default-info-list">
                            {% for doc in item.documents %}
                                <li><a href="{{doc.url}}">{{doc.title}}</a></li>
                            {% endfor %}
                        </ul>
                    </div>
                    {% endfor %}
                </div>
            </section>
        </main>