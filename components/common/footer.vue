<template>
    <footer class="footer">
        <div class="container">
            <div class="footer__content">
                <div class="footer-logo">
                    <img src="../../assets/icons/footer-logo.svg"
                        alt="logo">
                </div>
                <div class="footer__item">
                    <h3 class="footer__item-title">Menu</h3>
                    <ul class="footer__item-list">
                        <li>
                            <nuxt-link to="/solutions">Solutions</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/company">Company</nuxt-link>
                        </li>
                        <li>
                            <nuxt-link to="/contacts">Contacts</nuxt-link>
                        </li>
                    </ul>
                </div>
                <div class="footer__item">
                    <h3 class="footer__item-title">Contacts</h3>
                    <ul class="footer__item-list">
                        <li>
                            <a href="#">hello@parqour.com</a>
                        </li>
                        <li>
                            <a href="#">+1 516 468 1202</a>
                        </li>
                    </ul>
                </div>
                <div class="footer__item">
                    <h3 class="footer__item-title">Follow Us</h3>
                    <ul class="footer__item-list">
                        <li>
                            <a href="#">Facebook</a>
                        </li>
                        <li>
                            <a href="#">LinkedIn</a>
                        </li>
                    </ul>
                </div>
            </div>
            <h3 class="footer__copyright">
                Smart Parking Technologies© 2020 All rights reserved
            </h3>
        </div>
    </footer>
</template>

<script></script>


<style lang="scss" scoped>
$white-text: #ffffff;
$raleway: 'Raleway', sans-serif;
$primary-color: #00FF91;
$light-text: #222222;

.footer {
    padding-top: 110px;


    &__content {
        display: flex;
        align-items: flex-start;
        justify-content: space-around;
        padding-bottom: 40px;
        gap: 40px;
        flex-wrap: wrap;
    }

    &-logo {
        width: 150px;
        object-fit: cover;
    }

    &__item {
        display: flex;
        flex-direction: column;
        gap: 24px;

        &-title {
            font-weight: 700;
            font-size: 16px;
            line-height: 16px;
            color: $light-text;
        }

        &-list {
            display: flex;
            flex-direction: column;
            gap: 8px;

            a {
                font-weight: 400;
                font-size: 16px;
                line-height: 24px;
                color: $light-text;
            }
        }
    }

    &__copyright {
        text-align: center;
        padding: 32px 0px;
        border-top: 1px solid rgba(0, 0, 0, 0.2);
        font-weight: 400;
        font-size: 15px;
        line-height: 27px;
        color: $light-text;
    }
}
</style>