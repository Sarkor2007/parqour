<template>
    <div class="page">
        <header class="header">
            <div class="container">
                <div class="header__top">
                    <div class="header-logo">
                        <img src="../assets/icons/logo.svg"
                            alt="logo">
                    </div>
                    <nav class="header__nav">
                        <ul>
                            <li class="header__nav-item">
                                <a href="">Home</a>
                            </li>
                            <li class="header__nav-item">
                                <a href="">Solutions</a>
                            </li>
                            <li class="header__nav-item">
                                <a href="">Company</a>
                            </li>
                            <li class="header__nav-item">
                                <a href="">Contacts</a>
                            </li>
                        </ul>
                    </nav>
                </div>
                <main class="header__main">
                    <h1 class="header__main-title">
                        Shift your parking operation into top gear.
                    </h1>
                    <h3 class="header__main-subtitle">
                        Parqour is a software platform that simplifies parking operations and improves the customer
                        experience.
                        It
                        offers real-time data, automated plate recognition, and contactless payments.
                    </h3>
                    <button class="header__main-btn btn-primary">
                        Book a demo
                    </button>
                    <div class="header__box">
                        <div class="header__box-item">
                            <div class="header__box-img">
                                <img src="../assets/icons/planet.svg"
                                    alt="planet">
                            </div>
                            <div class="header__box-info">
                                <h3 class="header__box-title">22</h3>
                                <p class="header__box-text">Countries</p>
                            </div>
                        </div>
                        <div class="header__box-item">
                            <div class="header__box-img">
                                <img src="../assets/icons/parking.svg"
                                    alt="planet">
                            </div>
                            <div class="header__box-info">
                                <h3 class="header__box-title">+300</h3>
                                <p class="header__box-text">Parking areas</p>
                            </div>
                        </div>
                        <div class="header__box-item">
                            <div class="header__box-img">
                                <img src="../assets/icons/car.svg"
                                    alt="planet">
                            </div>
                            <div class="header__box-info">
                                <h3 class="header__box-title">+100M</h3>
                                <p class="header__box-text">Vehicles</p>
                            </div>
                        </div>
                    </div>
                </main>
            </div>
        </header>
        <div class="main-banner container">
            <img src="../assets/image/banner-bg.jpg"
                alt="banner">
        </div>

        <div class="partners container">
            <swiper :slidesPerView="5"
                :modules="modules"
                :autoplay="{
                    delay: 2500,
                    disableOnInteraction: false,
                }"
                class="mySwiper">
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
                <swiper-slide>
                    <img src="../assets/image/company.png"
                        alt="company">
                </swiper-slide>
            </swiper>
        </div>

        <section class="video">
            <h1 class="video-title">
                Meet the solution that is
                transforming the parking
                industry!
            </h1>
            <div class="video-box">
                <img src="../assets/image/video-image.jpg"
                    alt="video imaage">
                <a class="video-btn"
                    href="">
                    <img draggable="false"
                        src="../assets/image/play-btn.png"
                        alt="play">
                </a>
            </div>
        </section>

        <section class="whyus container">
            <div class="whyus__left">
                <h2 class="whyus__left-title">
                    Why Parqour?
                </h2>
                <div class="whyus__left-texts">
                    <p>Parqour offers a comprehensive end-to-end management platform to
                        increase revenue, reduce operational cost and enhance transparency.</p>
                    <p>Say goodbye to piecing together different vendors and integrations.
                        No need to spend huge capital on bulky hardware. Control all
                        operations from one platform.</p>
                    <p>Contactless parking and online payment methods makes the parking
                        experience easier for your customers too. The end result: higher
                        utilization and lower operating costs.</p>
                </div>
                <ul class="whyus__facts">
                    <li class="whyus__facts-item">99,6% license plate recognition rate</li>
                    <li class="whyus__facts-item">Online QR payment & 3rd party APIs
                        <p>(integrated with Parkmobile, SpotHero, Honk, PayByPhone)</p>
                    </li>
                    <div class="whyus__facts-item">
                        Data analytics
                        <p>(real-time occupancy, revenue, utilization, parking trends)</p>
                    </div>
                    <div class="whyus__facts-item">
                        Validation and permit management
                        <p>(free flow access for approved drivers)</p>
                    </div>
                    <div class="whyus__facts-item">
                        24/7 remote control system
                    </div>
                    <div class="whyus__facts-item">
                        Hardware with zero upfront costs
                    </div>
                    <div class="whyus__facts-item">
                        Zoning and violation detection
                        <p>(control POD, VIP and nested zones)</p>
                    </div>
                </ul>
            </div>
            <div class="whyus__right">
                <h1 class="whyus__right-title">How does it work?</h1>
                <h4 class="whyus__right-subtitle">
                    Use case: gated/gate-less paid parking
                </h4>
                <ul class="whyus__list">
                    <li class="whyus__list-item">
                        <h3 class="whyus__list-title">
                            Drive-in
                        </h3>
                        <p class="whyus__list-text">
                            The license plate is automatically detected and the
                            system starts parking session
                        </p>
                    </li>
                    <li class="whyus__list-item">
                        <h3 class="whyus__list-title">
                            Park & register
                        </h3>
                        <p class="whyus__list-text">
                            First time visitors will be instructed to scan QR and
                            register once
                        </p>
                    </li>
                    <li class="whyus__list-item">
                        <h3 class="whyus__list-title">
                            Drive-out
                        </h3>
                        <p class="whyus__list-text">
                            Driver is charged automatically
                        </p>
                    </li>
                </ul>
            </div>
        </section>

        <section class="slider">
            <div class="container">
                <div class="slider__head">
                    <div class="slider__head-img">
                        <img src="../assets/icons/logo-icon.svg"
                            alt="logo">
                    </div>
                    <div class="slider__head-title">
                        Get all-in-one with Parqour
                    </div>
                </div>

                <div class="slider__content">
                    <swiper :slidesPerView="3.5"
                        :spaceBetween="40"
                        :navigation="true"
                        :modules="modules"
                        class="mySwiper">
                        <swiper-slide>
                            <div class="slider__content-item">
                                <img class="slider__content-icon"
                                    src="../assets/icons/slider-icons/icon.svg"
                                    alt="slider icon">
                                <h3 class="slider__content-title">Satisfied <br> customers</h3>
                                <p class="slider__content-text">No tickets, barcodes or long
                                    lines. Just quick, free flow
                                    parking parking experience</p>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slider__content-item">
                                <img class="slider__content-icon"
                                    src="../assets/icons/slider-icons/icon.svg"
                                    alt="slider icon">
                                <h3 class="slider__content-title">Satisfied <br> customers</h3>
                                <p class="slider__content-text">No tickets, barcodes or long
                                    lines. Just quick, free flow
                                    parking parking experience</p>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slider__content-item">
                                <img class="slider__content-icon"
                                    src="../assets/icons/slider-icons/icon.svg"
                                    alt="slider icon">
                                <h3 class="slider__content-title">Satisfied <br> customers</h3>
                                <p class="slider__content-text">No tickets, barcodes or long
                                    lines. Just quick, free flow
                                    parking parking experience</p>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slider__content-item">
                                <img class="slider__content-icon"
                                    src="../assets/icons/slider-icons/icon.svg"
                                    alt="slider icon">
                                <h3 class="slider__content-title">Satisfied <br> customers</h3>
                                <p class="slider__content-text">No tickets, barcodes or long
                                    lines. Just quick, free flow
                                    parking parking experience</p>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slider__content-item">
                                <img class="slider__content-icon"
                                    src="../assets/icons/slider-icons/icon.svg"
                                    alt="slider icon">
                                <h3 class="slider__content-title">Satisfied <br> customers</h3>
                                <p class="slider__content-text">No tickets, barcodes or long
                                    lines. Just quick, free flow
                                    parking parking experience</p>
                            </div>
                        </swiper-slide>
                        <swiper-slide>
                            <div class="slider__content-item">
                                <img class="slider__content-icon"
                                    src="../assets/icons/slider-icons/icon.svg"
                                    alt="slider icon">
                                <h3 class="slider__content-title">Satisfied <br> customers</h3>
                                <p class="slider__content-text">No tickets, barcodes or long
                                    lines. Just quick, free flow
                                    parking parking experience</p>
                            </div>
                        </swiper-slide>
                    </swiper>
                </div>
            </div>

        </section>

        <section class="half">
            <div class="half-bg first"></div>
            <div class="container">
                <div class="half-wrapper">
                    <div class="half__content">
                        <h1 class="half__content-title">
                            Parqour for
                            gated parking
                        </h1>
                        <p class="half__content-text">
                            <b> Entry</b> - Transients enter without tickets. No need to
                            register before entering the parking facility. The
                            system automatically recognizes the license plate and
                            starts the parking session. Drivers with reservations
                            through platforms like ParkMobile, SpotHero,
                            PayByPhone or Honk enter the parking seamlessly
                            without scanning a barcode and tickets.
                        </p>
                        <p class="half__content-text">
                            <b> Payment</b> – users have numerous payment options:
                        <ul class="half__content-options">
                            <li>
                                <p><b> Online/web based app</b> - No need to download an
                                    app, users scan the QR code, that leads to a
                                    payment page</p>
                            </li>
                            <li>
                                <p><b> Terminal payment </b> - cash, credit card, Apple Pay,
                                    Google Pay</p>
                            </li>
                        </ul>
                        </p>
                        <p class="half__content-text">
                            <b> Exit</b> – The license plate is detected and the session
                            ends
                        </p>
                        <div class="half__content-message">No tickets, no attendants, no lines!</div>
                        <button class="half__content-btn btn-primary">
                            Learn More
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <section class="half right-side">
            <div class="half-bg second"></div>
            <div class="container">
                <div class="half-wrapper">
                    <div class="half__content">
                        <h1 class="half__content-title">
                            Parqour for
                            gated parking
                        </h1>
                        <p class="half__content-text">
                            <b> Entry </b> - Transients enter without barriers and tickets. The
                            system automatically captures the license plate and starts the
                            billing session.
                        </p>
                        <p class="half__content-text">
                            <b> Payment</b> - First time visitors are instructed to scan QR code
                            and register in the system by entering their license plate and
                            adding preferred payment methods (credit card,
                            Apple/Google pay).
                        </p>
                        <p class="half__content-text">
                            <b> Exit</b> - Registered drivers are charged automatically from a
                            credit card for the duration of their stay.
                        </p>
                        <div class="half__content-message">Returning drivers can enter and exit seamlessly, the system
                            charges them automatically on exit.</div>
                        <button class="half__content-btn btn-primary">
                            Learn More
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <section class="half">
            <div class="half-bg third"></div>
            <div class="container">
                <div class="half-wrapper">
                    <div class="half__content">
                        <h1 class="half__content-title">
                            Parqour for
                            valet parking
                        </h1>
                        <p class="half__content-text">
                            <b> Parking</b> - Camera automatically captures the license
                            plate at the entry
                        </p>
                        <p class="half__content-text">
                            <b> Check-in</b> - easy driver registration and communication
                            via SMS
                        </p>
                        <p class="half__content-text">
                            <b> Payment</b> - Customers pay with one touch via a mobile
                            app – compatible with Apple Pay and Google Pay.
                        </p>
                        <p class="half__content-text">
                            <b> Exit</b> - The license plate is recorded and the session
                            ends
                        </p>
                        <div class="half__content-message">Enhance transparency of financial flows and control
                            operations from one platform.</div>
                        <button class="half__content-btn btn-primary">
                            Learn More
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <section class="half right-side">
            <div class="half-bg fourth"></div>
            <div class="container">
                <div class="half-wrapper">
                    <div class="half__content">
                        <h1 class="half__content-title">
                            Parqour for
                            parking validation
                            & permit
                            management
                        </h1>
                        <p class="half__content-text">
                            <b> Use cases: </b> employee and tenant parking, monthly permit
                            management - seamless access for monthly parkers and drivers with
                            reservations made by third party platforms
                        <ul class="half__content-options">
                            <li>
                                <p><b> Entry </b>- The system checks the license plate and status of the
                                    permit</p>
                            </li>
                            <li>
                                <p><b> Exit</b> - All entry-exit events are logged and displayed in reports
                                </p>
                                <div class="options__items">
                                    <h3 class="options__items-item">
                                        No more hang tags, RFID cards and barcode scanning
                                    </h3>
                                    <h3 class="options__items-item">
                                        Integrated with all major reservation platforms (SpotHero,
                                        ParkMobile, Honk, PayByPhone etc.)
                                    </h3>
                                </div>

                            </li>
                        </ul>
                        </p>
                        <div class="half__content-message">Parking validation</div>
                        <p class="half__content-text">
                            <b> Use cases:</b> parking validation for hotel, restaurant, shopping mall,
                            fitness club, hospital visitors etc.
                        </p>

                        <p class="half__content-text">
                            <b> Via dashboard.</b> Company/Hotel/Restaurant administrators can
                            validate the parking session by entering the license plate to the
                            system using a web based dashboard. Access period can be
                            customized.
                        </p>
                        <p class="half__content-text">
                            <b> Via</b> promo code. Company administrator/receptionist distribute
                            promo codes, hotel, restaurant guests easily add the code to their
                            account by scanning the QR code.
                        </p>

                        <button class="half__content-btn btn-primary">
                            Learn More
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <section class="answers">
            <div class="answers-wrapper">
                <h1 class="answers-title">Frequently asked questions</h1>
                <div class="answers__content">
                    <ul class="akkordeon__list">
                        <li v-for="(item, index) in akkordeonList"
                            :key="index"
                            :class="{ active: item.active }"
                            class="akkordeon__item">
                            <div @click="changeActive(item)"
                                :class="{ active: item.active }"
                                class="akkordeon__item-head">
                                <h3>{{ item.header }}</h3>
                            </div>
                            <div :class="{ active: item.active }"
                                class="akkordeon__item-content">
                                <div class="akkordeon__item-text">
                                    {{ item.content }}
                                </div>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="blue__banner">
            <div class="container">
                <h1 class="blue__banner-title">
                    Ready to get
                    started?
                </h1>
                <button class="blue__banner-btn btn-primary">Book a Demo</button>
            </div>
        </section>

        <section class="about">
            <div class="about-bg"></div>
            <div class="container">
                <div class="about__content">
                    <div class="about__content-img">
                        <img src="../assets/icons/logo-icon.svg"
                            alt="logo">
                    </div>
                    <h1 class="about__content-title">
                        About us
                    </h1>
                    <p class="about__content-text">Car parks often provide the first impression of a destination. We focus
                        on transforming the parking customer
                        experience into one that is a welcome part of any journey.</p>
                    <p class="about__content-text">We are a global technology company with extended expertise and experience
                        in parking management, proptech,
                        smart city and smart parking technologies.</p>
                    <p class="about__content-text">Founded in 2020, Parqour already has more than 150 employees. It is
                        headquartered in the USA with offices or
                        representatives in 22 countries across Europe, the Middle-East, Central Asia and South-East Asia.
                    </p>
                </div>
            </div>
        </section>

        <footer class="footer">
            <div class="container">
                <div class="footer__content">
                    <div class="footer-logo">
                        <img src="../assets/icons/footer-logo.svg"
                            alt="logo">
                    </div>
                    <div class="footer__item">
                        <h3 class="footer__item-title">Menu</h3>
                        <ul class="footer__item-list">
                            <li>
                                <a href="#">Solutions</a>
                            </li>
                            <li>
                                <a href="#">Company</a>
                            </li>
                            <li>
                                <a href="#">Contacts</a>
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
    </div>
</template>

<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';

import { Autoplay, Navigation } from 'swiper';

const modules = ref([Autoplay, Navigation]);

let akkordeonList = ref([
    {
        active: false,
        header: "What if I already have barrier gates?",
        content: "Parqour can work with any type of barrier gates. In case of outdated gates andinfrastructure we will replace them.",
    },
    {
        active: false,
        header: 'How does the trial period work?',
        content: "Parqour can work with any type of barrier gates. In case of outdated gates andinfrastructure we will replace them.",
    },
    {
        active: false,
        header: 'What is the term of the trial period?',
        content: "Parqour can work with any type of barrier gates. In case of outdated gates andinfrastructure we will replace them.",
    },
    {
        active: false,
        header: 'How does Parqour earn money?',
        content: "Parqour can work with any type of barrier gates. In case of outdated gates andinfrastructure we will replace them.",
    },
    {
        active: false,
        header: 'What do Parqour’s investments cover?',
        content: "Parqour can work with any type of barrier gates. In case of outdated gates andinfrastructure we will replace them.",
    }
])

interface Item {
    active: boolean;
}


const changeActive = (item: Item) => {
    item.active = !item.active
}

</script>


<style lang="scss" scoped>
$white-text: #ffffff;
$raleway: 'Raleway', sans-serif;
$primary-color: #00FF91;
$light-text: #222222;

.btn-primary {
    background: $primary-color;
    border-radius: 4px;
    padding: 11px 24px 12px;
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;
    text-align: center;
}

.header {
    background: #0D76F4;
    background-image: url('../assets/image/main-bg.png');
    background-position: right center;
    background-size: contain;
    background-repeat: no-repeat;
    min-height: 850px;

    &__nav {
        position: absolute;
        left: 50%;
        transform: translateX(-50%);

        ul {
            display: flex;
            align-items: center;
            gap: 56px;
        }

        &-item {
            a {
                font-weight: 500;
                font-size: 16px;
                line-height: 24px;
                color: $white-text;
            }
        }
    }

    &__top {
        padding: 32px 0px;
        display: flex;
        align-items: center;
        position: relative;
    }

    &__main {
        max-width: 710px;
        margin: 30px auto;
        display: flex;
        flex-direction: column;
        align-items: center;

        &-title {
            font-family: $raleway;
            font-weight: 700;
            font-size: 56px;
            line-height: 64px;
            text-align: center;
            color: $white-text;
        }

        &-subtitle {
            margin-top: 24px;
            font-family: $raleway;
            font-weight: 400;
            font-size: 16px;
            line-height: 24px;
            text-align: center;
            color: #FFFFFF;
        }

        &-btn {
            color: #0D76F4;
            margin-top: 32px;
        }
    }

    &__box {
        margin-top: 64px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        width: 90%;

        &-item {
            display: flex;
            align-items: center;
            gap: 16px;
        }

        &-img {
            width: 64px;
            height: 64px;
            border: 2px solid $primary-color;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        &-info {
            display: flex;
            flex-direction: column;
        }

        &-title {
            font-weight: 600;
            font-size: 32px;
            line-height: 36px;
            color: $white-text;
        }

        &-text {
            font-family: $raleway;
            font-weight: 400;
            font-size: 16px;
            line-height: 24px;
            color: $white-text;
        }
    }
}

.main-banner {
    position: relative;

    img {
        padding: 0px 12px;
        left: 0;
        width: 100%;
        border-radius: 24px;
        position: absolute;
        transform: translateY(-50%);
    }
}

.partners {
    margin-top: 300px;
    padding: 20px 12px;

    .swiper {
        width: 100%;
        height: 100%;
    }

    .swiper-slide {
        text-align: center;
        font-size: 18px;
        background: #fff;

        /* Center slide text vertically */
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .swiper-slide img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
}

.video {
    max-width: 965px;
    margin: auto;
    width: 100%;
    margin-top: 40px;

    &-title {
        font-weight: 500;
        font-size: 45px;
        line-height: 67px;
        max-width: 610px;
        margin: auto;
        text-align: center;
        color: $light-text;
    }

    &-box {
        margin-top: 90px;
        position: relative;

        &::before {
            content: '';
            position: absolute;
            left: -65px;
            top: -60px;
            width: 246px;
            height: 246px;
            background-color: $primary-color;
        }

        &::after {
            content: '';
            position: absolute;
            bottom: -30px;
            right: 10px;
            width: 246px;
            height: 246px;
            background-image: url('../assets/image/cutted-square.png');
        }
    }

    &-btn {
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);

        img {
            user-select: none;
        }
    }
}

.whyus {
    margin-top: 100px;
    padding-bottom: 30px;
    display: flex;
    justify-content: space-between;

    &__left {
        width: 46%;

        &-title {
            font-weight: 500;
            font-size: 64px;
            line-height: 67px;
            color: $light-text;
        }

        &-texts {
            margin-top: 36px;
            width: 100%;
            display: flex;
            flex-direction: column;
            gap: 30px;

            p {
                font-weight: 400;
                font-size: 15px;
                line-height: 27px;
                color: $light-text;
            }
        }
    }

    &__facts {
        margin-top: 35px;
        width: 100%;
        display: flex;
        flex-direction: column;
        gap: 24px;

        &-item {
            font-weight: 400;
            font-size: 15px;
            line-height: 18px;
            color: $light-text;
            padding-left: 30px;
            position: relative;

            &::before {
                content: '';
                position: absolute;
                width: 13px;
                height: 13px;
                background-color: $primary-color;
                left: 0;
                top: 2px;
            }
        }

        p {
            font-weight: 400;
            font-size: 9px;
            line-height: 17px;
        }
    }

    &__right {
        width: 45%;

        &-title {
            font-weight: 500;
            font-size: 51.2px;
            line-height: 54px;
            color: $light-text;
        }

        &-subtitle {
            font-weight: 400;
            font-size: 15px;
            line-height: 27px;
            color: $light-text;
            margin-top: 36px;
        }
    }

    &__list {
        display: flex;
        flex-direction: column;
        margin-top: 50px;
        border: 1px solid rgba(0, 0, 0, 0.1);
        position: relative;

        &::before,
        &::after {
            position: absolute;
            content: '';
            z-index: 0;
            width: 15px;
            height: 15px;
            background-color: $primary-color;
        }

        &::before {
            top: -30px;
            left: -1px;
        }

        &::after {
            left: -16px;
            top: -15px;
        }

        &-item {
            padding: 16px;
        }

        &-item:not(:last-child) {
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
        }

        &-title {
            font-weight: 400;
            font-size: 24px;
            line-height: 36px;
            color: $light-text;
        }

        &-text {
            font-weight: 400;
            font-size: 15px;
            line-height: 27px;
            color: $light-text;
        }
    }
}

.slider {
    margin-top: 100px;
    background: $light-text;
    padding: 20px;
    padding-bottom: 0px;
    position: relative;

    &::before {
        content: '';
        position: absolute;
        background-image: url('../assets/image/cutted-square-two.png');
        width: 246px;
        height: 246px;
        background-size: cover;
        left: -20px;
        top: -90px;
    }

    &::after {
        content: '';
        position: absolute;
        width: 40px;
        height: 40px;
        background-color: $primary-color;
        right: 0;
        top: -40px;
    }

    &__head {
        padding-left: 36px;
        padding-top: 40px;

        &-title {
            margin-top: 12px;
            font-weight: 500;
            font-size: 44px;
            line-height: 67px;
            color: $white-text;
        }
    }

    &__content {
        margin-top: 70px;

        .swiper {
            position: relative;
            right: -10%;
            width: 100%;
            height: 100%;
            padding-top: 110px;
            transform: translateY(-110px);
        }

        .swiper-slide {
            background: $white-text;
            border: 1px solid rgba(0, 0, 0, 0.1);
            border-radius: 5px;
            display: flex;
            justify-content: center;
            min-height: 410px;
        }

        &-item {
            width: 100%;
            height: 100%;
            padding: 32px 36px;
        }

        &-icon {
            width: 63px;
            height: 63px;
            object-fit: contain;
        }

        &-title {
            margin-top: 60px;

            font-weight: 400;
            font-size: 24px;
            line-height: 36px;
            color: $light-text;
        }

        &-text {
            margin-top: 16px;
            font-weight: 400;
            font-size: 15px;
            line-height: 27px;
            color: $light-text;
        }
    }
}

.half {
    position: relative;
    width: 100%;
    min-height: 810px;

    &-bg {
        position: absolute;
        left: 0;
        bottom: 0;
        z-index: 0;
        width: 50%;
        height: 100%;
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;

        &.first {
            background-image: url('../assets/image/image-1.jpg');
        }

        &.second {
            background-image: url('../assets/image/image-2.jpg');
        }

        &.third {
            background-image: url('../assets/image/image-3.jpg');
        }

        &.fourth {
            background-image: url('../assets/image/image-4.jpg');
        }


        &::after {
            position: absolute;
            content: '';
            bottom: 0;
            right: 0;
            z-index: 0;
            width: 40px;
            height: 40px;
            background-color: $primary-color;
        }
    }

    &-wrapper {
        width: 100%;
        display: flex;
        min-height: 800px;
        justify-content: flex-end;
        align-items: center;
    }

    &__content {
        width: 50%;
        padding: 36px 50px;

        &-title {
            font-weight: 500;
            font-size: 64px;
            line-height: 67px;
            color: $light-text;
        }

        p {
            margin-top: 28px;
            font-weight: 500;
            font-size: 15px;
            line-height: 27px;
            color: $light-text;

            b {
                font-weight: 700;
            }
        }

        &-options {
            margin-top: 25px;
            display: flex;
            flex-direction: column;
            gap: 8px;
            width: 100%;
            padding-left: 30px;

            p {
                margin-top: 0px;
            }
        }

        .options__items {
            margin-top: 8px;
            padding-left: 30px;

            h3 {
                margin-top: 2px;
                font-weight: 400;
                font-size: 14px;
                line-height: 24px;
                color: $light-text;
            }
        }

        &-message {
            margin-top: 30px;
            font-weight: 700;
            font-size: 15px;
            line-height: 27px;
            color: $light-text;
        }

        &-btn {
            margin-top: 30px;
            color: #157FFF;
        }
    }

    &.right-side {
        position: relative;

        &::after {
            content: '';
            width: 40px;
            height: 40px;
            background-color: $primary-color;
            position: absolute;
            left: 0;
            bottom: 0;
        }

        .half-wrapper {
            justify-content: flex-start;
        }

        .half-bg {
            left: auto;
            right: 0;

            &:after {
                top: 0;
                left: 0;
                width: 246px;
                height: 246px;
                background-color: transparent;
                background-size: cover;
                background-image: url('../assets/image/cutted-square-two.png');
            }
        }

        .half__content {
            padding-top: 55px;
        }
    }

    &:last-child {
        min-height: 1000px;

        .half-wrapper {
            min-height: 1000px;
            align-items: flex-start;
        }

        .half__content {
            padding-top: 20px;
            padding-left: 0;
        }
    }

}

.answers {
    background: #F6F6F6;
    position: relative;

    &::after {
        content: '';
        position: absolute;
        background-image: url('../assets/image/cutted-square.png');
        width: 246px;
        height: 246px;
        background-position: center;
        background-size: contain;
        bottom: -80px;
        right: 0;
    }

    .answers-wrapper {
        padding: 90px 0px 80px;
        max-width: 756px;
        width: 100%;
        margin: auto;
    }

    &-title {
        font-weight: 500;
        font-size: 44px;
        line-height: 67px;
        text-align: center;
        color: $light-text;
    }

    &__content {
        margin-top: 55px;
    }

    .akkordeon {
        &__list {
            display: flex;
            flex-direction: column;
        }

        &__item {
            position: relative;

            &::after {
                position: absolute;
                content: '';
                top: 0;
                left: -1562.5rem;
                width: 50000px;
                height: 100%;
                transition: .3s all;
                background-color: $primary-color;
                opacity: 0;
            }

            &.active {

                &::after {
                    opacity: 1;
                    transition: .3s all;
                }


            }

            &-head {
                position: relative;
                z-index: 1;
                cursor: pointer;
                padding: 22px 0px 24px;
                border-bottom: 1px solid #979797;
                position: relative;
                display: flex;
                align-items: center;

                h3 {
                    font-weight: 400;
                    font-size: 23px;
                    line-height: 25px;
                    color: $light-text;
                }

                &.active {
                    border-bottom: none;

                    &::after {
                        transition: .3s all;
                        transform: rotate(90deg);
                    }
                }

                &::after {
                    content: "";
                    background-image: url('../assets/icons/arrow.svg');
                    background-position: center;
                    background-size: cover;
                    position: absolute;
                    right: 20px;
                    width: 6px;
                    height: 12px;
                    object-fit: contain;
                    transition: .3s all;

                }

            }

            &-content {
                position: relative;
                z-index: 1;
                max-height: 0;
                overflow: hidden;
                transition: max-height 0.3s;

                &.active {
                    transition: max-height .6s;
                    max-height: 500px;
                }
            }

            &-text {
                padding: 30px 0px 40px;
            }
        }
    }
}

.blue__banner {
    padding: 120px 0px 80px;
    position: relative;

    &::after {
        position: absolute;
        content: '';
        top: 0;
        left: 0;
        z-index: -1;
        width: calc(100% - 246px);
        height: 100%;
        background-color: #157FFF;
        background-image: url('../assets/image/bg-image.png');
        background-position: center right;
        background-size: auto 100%;
        background-repeat: no-repeat;
    }

    &-title {
        font-weight: 500;
        font-size: 64px;
        line-height: 67px;
        color: $white-text;
    }

    &-btn {
        margin-top: 26px;
        color: #157FFF;
    }
}

.about {
    padding: 80px 0px;
    position: relative;

    &-bg {
        background-image: url('../assets/image/about-bg.jpg');
        position: absolute;
        height: 100%;
        top: 0;
        right: 0;
        z-index: 0;
        background-position: center center;
        background-repeat: no-repeat;
        background-size: cover;
        width: calc(100% - ((100% - 1170px) / 2));
    }

    &__content {
        position: relative;
        z-index: 1;
        padding: 0px 80px;

        &-title {
            margin-top: 70px;
            font-weight: 500;
            font-size: 64px;
            line-height: 67px;
            color: $white-text;
        }

        &-text {
            margin-top: 36px;
            font-weight: 400;
            font-size: 15px;
            line-height: 27px;
            color: $white-text;
        }
    }
}

.footer {
    padding-top: 110px;

    .container {}

    &__content {
        display: flex;
        align-items: flex-start;
        justify-content: space-between;
        padding-bottom: 40px;
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

<style lang="scss">
.swiper-button-next::after,
.swiper-button-prev::after {
    content: '';
    width: 16px;
    height: 24px;
    object-fit: contain;
    background-image: url('../assets/icons/slider-arrow.svg');
}

.swiper-button-prev::after {
    transform: rotate(180deg);
}

.swiper-button-prev {
    top: 12px;
    right: 80px;
    left: auto;
}

.swiper-button-next {
    top: 12px;
    right: 40px;
    left: auto;
}
</style>