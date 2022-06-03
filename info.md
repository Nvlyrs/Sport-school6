---
layout: default
title: Сведения об организации
---
<main class="main">
            <section class="info-section">
                <div class="info-section__content-wrapper content-wrapper">
                    <h2 class="info-section__title default-section-title">Сведения об организации</h2>
                    <h3 class="info-section__card-title default-card-title">Нвигация по страцие</h3>
                    <ul class="info-section__navbar">
                        {% for item in site.data.organisation-info%}
                        <li><a href="#{{item.anchor}}">{{item.id}}. {{item.header}}</a></li>
                        {% endfor %}
                    </ul>
                    <div class="info-section__general" id="general">
                        <h3 class="info-section__card-title default-card-title">1.Основные сведения</h3>
                        <ul class="info-section__list default-info-list">
                            Органы, осуществляющие функции и полномочия учредителя:
                            <li>&mdash; Администрация Волгограда;</li>
                            <li>&mdash; Департамент по образованию администрации Волгограда;</li>
                            <li>&mdash; Комитет по физической культуре и спорту администрации Волгограда;</li>
                            <li>&mdash; Департамент муниципального имущества администрации Волгограда.</li>
                        </ul>
                        <div class="info-section__main default-paragraph">
                            <p class="info-paragraph">
                                <span>Юридический и фактический адреса: <br> </span>
                                <span>Контактный телефон: <a href="tel: +78442621730">+7(8442)62-17-30</a> <br> </span>
                                <span>Адресс электронной почты: <a
                                        href="mailto: MOUDUSSH.6@yandex.ru">MOUDUSSH.6@yandex.ru</a></span>
                            </p>
                            <p class="info-paragraph">
                                <span>Режим и график работы:</span>
                                <span>Понедельник-суббота: c <time>8:00</time> до <time>20:00</time></span>
                            </p>
                            <p class="info-paragraph">
                                <span>Администрация:</span>
                                <span>Понедельник-пятница: c <time>8:30</time> до <time>17:30</time></span>
                                <span>Перерыв: c <time>12:30</time> до <time>13:30</time></span>
                            </p>
                        </div>
                    </div>
                    {% for item in site.data.organisation-info%}
                    <div class="info-section__general" id="{{item.anchor}}">
                        <h3 class="info-section__card-title default-card-title">{{item.id}}. {{item.header}}</h3>
                        <div class="default-paragraph">
                            {% for paragraph in item.paragraphs%}
                                {% if paragraph.text != "" %}
                                    {% if paragraph.link != "" %}
                                        <p class="info-paragraph">
                                            {{paragraph.text}} <a href="{{paragraph.link}}" target="_blank">{{paragraph.linkName}}</a>
                                        </p>   
                                        {% else %} 
                                            <p class="info-paragraph">
                                                {{paragraph.text}} 
                                            </p>
                                    {% endif %}
                                {% endif %}
                            {% endfor %}
                        </div>
                        <ul class="info-section__list default-info-list">
                            {% for listItem in item.list%}
                                    {% if listItem.fileName != "" and listItem.name != "" %}
                                        <li>
                                            {{listItem.name}}: <a href="{{listItem.file}}" target="_blank">{{listItem.fileName}}</a>
                                        </li>
                                    {% else if listItem.name != "" %}
                                        <li>
                                            {{listItem.name}}
                                        </li>  
                                    {% endif %}     
                                    {% if listItem.fileName != "" and listItem.name == "" %}
                                        <li>
                                            <a href="{{listItem.file}}" target="_blank">{{listItem.fileName}}</a>
                                        </li>
                                    {% endif %}
                            {% endfor %}
                        </ul>
                    </div>
                    {% endfor %}
                </div>
            </section>
        </main>