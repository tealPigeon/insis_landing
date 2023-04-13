<template>
    <div class="landing">
        <section class="main">
            <div class="container main__container">

                <header class="header">
                    <img  class="header__logo" src="images/logo.svg" alt />
                    <div class="header__contact">8 800 250 60 60</div>
                </header>

                <div class="main__wrapper">
                    <div class="main__title__wrapper">
                        <h1 class="title-h1">
                            За
                            <span class="green">разумное</span> потребление
                        </h1>

                        <div class="main__subtitle__wrapper">
                            <div class="dash"></div>

                            <div class="title-h3">
                                до
                                <b>100 Мбит/с</b> + от
                                <b>150 каналов</b>
                                <br />Первый месяц бесплатно
                            </div>
                        </div>

                        <button class="button" @click="scrollToFeedback">
                            Оставить заявку
                        </button>
                    </div>

                    <img class="main__image" src="images/earth.png" alt />
                    <img class="main__image__moble" src="images/earth_mobile.png" alt />

                </div>

            </div>
        </section>

        <section class="advantages">
            <div class="decoration_line"></div>
            <div class="container advantages__container">
                <div class="advantages__wrapper">
                    <img class="image" src="images/wallet.png" alt />
                    <div class="advantages__text">
                        <h2 class="white title-h2">
                            <b class="green">Не переплачивайте!</b> За то, что другие навязывают.
                        </h2>
                        <h3 class="title-h3">
                            <b>Рациональной потребление</b> – пользоваться тем, что действительно надо
                        </h3>
                    </div>
                </div>

                <div class="cards">
                    <div class="card">
                        <img class="card-img" src="images/speed.png" />
                        <div class="card-text">
                            Только
                            <br />
                            <span class="green">необходимая</span>
                            <br />скорость
                        </div>
                    </div>

                    <div class="card">
                        <img class="card-img" src="images/price.png" />
                        <div class="card-text">
                            Только
                            <br />
                            <span class="green">разумная</span>
                            <br />цена
                        </div>
                    </div>

                    <div class="card">
                        <img class="card-img" src="images/conditions.png" />
                        <div class="card-text">
                            Только
                            <br />
                            <span class="green">выгодные</span>
                            <br />условия
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="benefits">
            <div class="decoration_line"></div>
            <div class="container benefits__container">
                <h2 class="title-h2">
                    Интернет + Цифровое
                    <span class="green">ТВ</span>
                </h2>

                <h3 class="title-h3">Чистая выгода</h3>

                <div class="wrapper">
                    <div>
                        <img class="arrow__left-top" src="images/pointing_arrow.png" alt />
                        <div class="benefit benefit__left-top" style="">
                            <img src="images/application.png" alt />
                            <div class="benefit__text"><b>Приложение</b> Инсис ТВ</div>
                        </div>
                    </div>

                    <div>
                        <img class="arrow__right-top" style=""
                            src="images/pointing_arrow.png" alt />
                        <div class="benefit benefit__right-top" style="">
                            <img src="images/channels.png" alt />
                            <div class="benefit__text"><b>Хороший</b> выбор каналов</div>

                        </div>
                    </div>

                    <div>
                        <img class="arrow__left-bottom" style=""
                            src="images/pointing_arrow.png" alt />
                        <div class="benefit benefit__left-bottom" style="">
                            <img src="images/speed_connection.png" alt />
                            <div class="benefit__text"><b>Быстрое</b> подключение </div>
                        </div>

                    </div>

                    <div>
                        <img class="arrow__right-bottom" style=""
                            src="images/pointing_arrow.png" alt />
                        <div class="benefit benefit__right-bottom" style="">
                            <img src="images/tech-support.png" alt />
                            <div class="benefit__text">Надежная тех.поддержка в <b>любое время</b></div>
                        </div>

                    </div>

                    <img class="image" src="images/computer.png" alt />
                </div>
            </div>
        </section>

        <section class="feedback">
            <div class="decoration_line_green"></div>

            <div class="container feedback__container">
                <div class="feedback__wrapper">
                    <div>
                        <h2 class="white title-h2">
                            Остались
                            <br />вопросы?
                        </h2>

                        <h3 class="title-h3 white">Оставляй заявку</h3>

                        <img class="feedback__arrow desktop" src="images/arrow.svg" alt />
                    </div>

                    <div>
                        <h3 class="title-h3 white desktop">Объясняем понятно, решаем быстро</h3>

                        <form ref="feedback" class="feedback__form" @submit.prevent="submit">

                            <div class="feedback__input__wrapper">
                                <input class="feedback__input" placeholder="+7 (___) ___-__-__" v-mask="'+7 (###) ###-##-##'" v-model="number" type="text" id="phone" name="phone" />
                            </div>

                            <button type="submit" class="button">
                                Перезвоните мне
                            </button>
                        </form>

                        <p class="privacy-politic">
                            Нажимая на кнопку «Перезвоните мне», вы даёте
                            согласие на обработку персональных данных
                        </p>
                    </div>
                </div>

                <hr />

                <footer class="footer">
                    <div class="footer__copyright">
                        <img class="footer__logo" src="images/white_logo.svg" alt />
                        <p class="footer__copyright__text">2007-2022 год</p>
                    </div>

                    <div class="footer-social-networks" style>
                        <p class="footer-social-networks__text">Мы в соц. сетях:</p>
                        <div>
                            <a href="https://vk.com/">
                                <img class="social-network" src="images/vk.svg" alt />
                            </a>

                            <a href="https://www.youtube.com/">
                                <img class="social-network" src="images/youtube.svg" alt />
                            </a>
                        </div>
                    </div>

                    <div class="footer-contacts">
                        <p class="footer-contacts__phone">8-800-250-60-60</p>
                        <p class="footer-contacts__email">info@profintel.ru</p>
                    </div>
                </footer>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: "IndexPage",

    data: function () {
        return {
            number: ""
        };
    },

    methods: {
        submit() {
            console.log(this.number);
        },

        scrollToFeedback() {
            this.$refs["feedback"].scrollIntoView({ behavior: "smooth" });
        }
    }
};
</script>


