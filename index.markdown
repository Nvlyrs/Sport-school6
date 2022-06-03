---
layout: default
title: Главная
content: materials-content
---
<main class="main">
            <section class="main-section">
                <div class="main-section__gradient"></div>
                <img src="../assets/img/main-section-image.jpg" alt="" class="main-section__imgb imgb">
                <div class="main-section__content-wrapper content-wrapper">
                    <h1 class="main-section__title default-section-title">МБУ СШ №6</h1>
                    <h3 class="main-section__subtitle default-card-title">МУНИЦИПАЛЬНОЕ БЮДЖЕТНОЕ УЧРЕЖДЕНИЕ СПОРТИВНАЯ
                        ШКОЛА № 6 Г. ВОЛГОГРАДА.<br>
                        ОСНОВАНО В 1960 ГОДУ.</h3>
                </div>
                <div class="main-section__decoration">
                    <img src="../assets/img/gymnast.png" alt="" class="main-section__gymnast">
                </div>
            </section>
            <section class="kind-of-sports-section parallax" id="kinds-of-sports">
                <div class="kind-of-sports-section__content-wrapper content-wrapper">
                    <h2 class="kind-of-sports-section__title default-section-title">Виды спорта</h2>
                    {% for item in site.data.kind-of-sports %}
                    <figure class="kind-of-sports-section__card card flex">
                        <div class="kind-of-sports-section__card-image card__image">
                            <img src="{{item.img}}" alt="" class="imgb">
                        </div>
                        <figcaption class="kind-of-sports-section__card-caption card__caption">
                            <h3 class="card__title default-card-title">{{item.header}}</h3>
                            <p class="card__paragraph default-paragraph">{{item.disc}}</p>
                        </figcaption>
                    </figure>
                    {% endfor %}
                </div>
            </section>
            <section class="news-section" id="news-section">
                <h2 class="news-section__title default-section-title">Новости</h2>
                <div class="swiper-news">
                    <div class="swiper-wrapper">
                        {% for item in site.data.news %}
                        <div class="news-card flex row swiper-slide">
                            <div class="news-card__image">
                                <img src="{{item.img}}" alt="" class="imgb">
                            </div>
                            <div class="news-card__text-body">
                                <h3 class="news-card__news-title default-card-title">{{item.header}}</h3>
                                <p class="news-card__news-desctiption default-paragraph">{{item.disc}}</p>
                            </div>
                        </div>
                        {% endfor %}
                    </div>
                    <div class="swiper-pagination"></div>
                </div>
            </section>
            <section class="coaches-section" id="coaches-section">
                <div class="coaches-section__background">
                    <img src="../assets/img/coaches/background-image.png" alt="" class="imgb">
                </div>
                <div class="coaches-section__content-wrapper content-wrapper">
                    <h2 class="coaches-section__title default-section-title">Сотрудники</h2>
                    <div class="swiper">
                        <div class="swiper-wrapper">
                            <div class="swiper-slide">
                                <div class="coaches-section__coach-card coach-card flex">
                                    <div class="coaches-section__kinds-of-sports coach-card__kinds-of-sports">
                                        <h3 class="coaches-section__card-title coach-card__title default-card-title">
                                            Виды
                                            спорта
                                        </h3>
                                        <ul
                                            class="coaches-section__kinds-of-sports-list coach-card__kinds-of-sports-list default-paragraph">
                                            <li
                                                class="coaches-section__kinds-of-sports-list-item coach-card__kinds-of-sports-list-item">
                                                &mdash; Спортивная гимнастика</li>
                                            <li
                                                class="coaches-section__kinds-of-sports-list-item coach-card__kinds-of-sports-list-item">
                                                &mdash; Спортивная акробатика</li>
                                            <li
                                                class="coaches-section__kinds-of-sports-list-item coach-card__kinds-of-sports-list-item">
                                                &mdash; Художественная гимнастика</li>
                                        </ul>
                                    </div>
                                    <div class="coaches-section__text-body coach-card__text-body flex">
                                        <h3 class="coaches-section__card-title coach-card__title default-card-title">
                                            Тимофеев
                                            Михаил
                                            Юрьевич</h3>
                                        <p
                                            class="coaches-section__card-description coach-card__description default-paragraph">
                                            Тренер по спортивной гимнастике. «Мастер спорта России» по спортивной
                                            гимнастике.
                                            Высшая
                                            квалификационная категория. Кандидат педагогических наук. Окончил
                                            Волгоградскую
                                            государственную академию физической культуры в 2006 году. Присуждена
                                            квалификация
                                            специалист по физической культуре и спорту по специальности «физическая
                                            культура
                                            и
                                            спорт». Стаж работы по специальности 13 лет.</p>
                                    </div>
                                    <img src="../assets/img/coaches/coach-id1.png" alt="фото_тренера"
                                        class="coaches-section__card-image coach-card__image">
                                </div>
                            </div>
                            <div class="swiper-slide">
                                <div class="coaches-section__coach-card coach-card flex">
                                    <div class="coaches-section__kinds-of-sports coach-card__kinds-of-sports">
                                        <h3 class="coaches-section__card-title coach-card__title default-card-title">
                                            Виды
                                            спорта
                                        </h3>
                                        <ul
                                            class="coaches-section__kinds-of-sports-list coach-card__kinds-of-sports-list">
                                            <li
                                                class="coaches-section__kinds-of-sports-list-item coach-card__kinds-of-sports-list-item">
                                                &mdash; Спортивная гимнастика</li>
                                            <li
                                                class="coaches-section__kinds-of-sports-list-item coach-card__kinds-of-sports-list-item">
                                                &mdash; Спортивная акробатика</li>
                                            <li
                                                class="coaches-section__kinds-of-sports-list-item coach-card__kinds-of-sports-list-item">
                                                &mdash; Художественная гимнастика</li>
                                        </ul>
                                    </div>
                                    <div class="coaches-section__text-body coach-card__text-body flex">
                                        <h3 class="coaches-section__card-title coach-card__title default-card-title">
                                            Тимофеев
                                            Михаил
                                            Юрьевич</h3>
                                        <p
                                            class="coaches-section__card-description coach-card__description default-paragraph">
                                            Тренер по спортивной гимнастике. «Мастер спорта России» по спортивной
                                            гимнастике.
                                            Высшая
                                            квалификационная категория. Кандидат педагогических наук. Окончил
                                            Волгоградскую
                                            государственную академию физической культуры в 2006 году. Присуждена
                                            квалификация
                                            специалист по физической культуре и спорту по специальности «физическая
                                            культура
                                            и
                                            спорт». Стаж работы по специальности 13 лет.</p>
                                    </div>
                                    <img src="../assets/img/coaches/coach-id1.png" alt="фото_тренера"
                                        class="coaches-section__card-image coach-card__image">
                                </div>
                            </div>
                        </div>
                        <div class="swiper-pagination"></div>
                        <div class="swiper-button-prev"></div>
                        <div class="swiper-button-next"></div>
                    </div>
                </div>
            </section>
            <section class="contacts-section" id="contacts-section">
                <div class="contacts-section__row flex">
                    <div class="contacts-section__text-body">
                        <h3 class="default-card-title contacts-section__label">МУНИЦИПАЛЬНОЕ БЮДЖЕТНОЕ УЧРЕЖДЕНИЕ
                            СПОРТИВНАЯ ШКОЛА № 6 Г.
                            ВОЛГОГРАДА</h3>
                        <div class="contacts-section__adress flex">
                            <img src="../assets/img/contacts-section/location.png" alt="">
                            <p class="contacts-section__paragraph default-paragraph">Адрес: <br> город Волгоград,
                                Красноармейский район, 400082 ул. им. Вучетича 29</p>
                        </div>
                        <div class="contacts-section__email flex">
                            <img src="../assets/img/contacts-section/mail.png" alt="">
                            <p class="contacts-section__paragraph default-paragraph">Email: <br> moudussh.6@yandex.ru
                            </p>
                        </div>
                    </div>
                    <div class="contacts-section__map" id="map"></div>
                </div>
            </section>
</main>