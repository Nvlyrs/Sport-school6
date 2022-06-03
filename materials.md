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
                        {% for item in site.data.organisation-info%}
                        <li><a href="#actual">{{item.id}}. {{item.header}}</a></li>
                        {% endfor %}
                        <li><a href="#corruption">2.Противодействие коррупции</a></li>
                    </ul>
                    <div class="info-section__actual" id="actual">
                        <h3 class="info-section__card-title default-card-title">1.Последние методические материалы</h3>
                        <div class="info-section__main default-paragraph">
                            <p>
                                30 декабря 2021 г. <br> <a href="">Программа спортивной подготовки по художественной
                                    гимнастике</a>;
                            </p>
                            <p>
                                30 декабря 2021 г. <br> <a href="">Программа спортивной подготовки по спортивной
                                    акробатике</a>;
                            </p>
                            <p>
                                30 декабря 2021 г. <br> <a href="">Программа спортивной подготовки по спортивной
                                    гимнастике</a>;
                            </p>
                            <p>
                                15 сентября 2017 г. <br> <a href="">Рабочая образовательная программа по спортивной
                                    гимнастике для юношей</a>;
                            </p>
                            <p>
                                31 августа 2016 г. <br> <a href="">Подготовительные упражнения для мальчиков младшего возраста в
                                спортивной гимнастике на отдельных видах многоборья (опорный прыжок и перекладина)</a>.
                            </p>
                        </div>
                    </div>
                    <div class="info-section__corruption" id="corruption">
                        <h3 class="info-section__card-title default-card-title">2.Противодействие коррупции</h3>
                        <ul class="default-info-list">
                            <li>&mdash; <a href="">Положение о противодействии коррупции положение; </a> </li>
                            <li>&mdash; <a href="">Положение антикоррупционной политики. </a></li>
                        </ul>
                    </div>
                </div>
            </section>
        </main>