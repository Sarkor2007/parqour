<template>
    <div @click="openVideo"
        :class="{ active: isOpenVideo }"
        class="filter"></div>
    <div class="partners container">
        <swiper :slidesPerView="3"
            :modules="modules"
            :autoplay="{
                delay: 2500,
                disableOnInteraction: false,
            }"
            :loop="true"
            :breakpoints="{
                992: {
                    slidesPerView: 5,
                },
                768: {
                    slidesPerView: 4,
                },
            }"
            class="mySwiper">
            <swiper-slide>
                <img src="../assets/image/companies/1.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/2.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/3.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/4.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/5.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/1.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/2.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/3.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/4.png"
                    alt="company">
            </swiper-slide>
            <swiper-slide>
                <img src="../assets/image/companies/5.png"
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
            <a @click="openVideo"
                class="video-btn">
                <img draggable="false"
                    src="../assets/image/play-btn.png"
                    alt="play">
            </a>
        </div>
        <div :class="{ active: isOpenVideo }"
            class="video__item">
            <iframe width="560"
                height="315"
                src="https://www.youtube.com/embed/ccqqaSQm6dc"
                title="YouTube video player"
                frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
                allowfullscreen></iframe>
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
                <swiper :slidesPerView="1"
                    :spaceBetween="40"
                    :navigation="true"
                    :modules="modules"
                    :loop="true"
                    :breakpoints="{
                        660: {
                            slidesPerView: 2,
                        },
                        992: {
                            slidesPerView: 3,
                        },
                        1100: {
                            slidesPerView: 3.5,
                        },
                    }"
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
                                src="../assets/icons/slider-icons/icon2.svg"
                                alt="slider icon">
                            <h3 class="slider__content-title">Reduce capital <br> expenses</h3>
                            <p class="slider__content-text">We can beat any PARCS’s
                                offer by 30% and up to 3
                                times</p>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="slider__content-item">
                            <img class="slider__content-icon"
                                src="../assets/icons/slider-icons/icon3.svg"
                                alt="slider icon">
                            <h3 class="slider__content-title">Increased <br> bottomline</h3>
                            <p class="slider__content-text">No tickets, barcodes or long
                                lines. Just quick, free flow
                                parking parking experience</p>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="slider__content-item">
                            <img class="slider__content-icon"
                                src="../assets/icons/slider-icons/icon4.svg"
                                alt="slider icon">
                            <h3 class="slider__content-title">Minimal <br> investment</h3>
                            <p class="slider__content-text">Our subscription plans let
                                you get started today with
                                little to no down payment.</p>
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
                                src="../assets/icons/slider-icons/icon2.svg"
                                alt="slider icon">
                            <h3 class="slider__content-title">Reduce capital <br> expenses</h3>
                            <p class="slider__content-text">We can beat any PARCS’s
                                offer by 30% and up to 3
                                times</p>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="slider__content-item">
                            <img class="slider__content-icon"
                                src="../assets/icons/slider-icons/icon3.svg"
                                alt="slider icon">
                            <h3 class="slider__content-title">Increased <br> bottomline</h3>
                            <p class="slider__content-text">No tickets, barcodes or long
                                lines. Just quick, free flow
                                parking parking experience</p>
                        </div>
                    </swiper-slide>
                    <swiper-slide>
                        <div class="slider__content-item">
                            <img class="slider__content-icon"
                                src="../assets/icons/slider-icons/icon4.svg"
                                alt="slider icon">
                            <h3 class="slider__content-title">Minimal <br> investment</h3>
                            <p class="slider__content-text">Our subscription plans let
                                you get started today with
                                little to no down payment.</p>
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
</template>

<script setup lang="ts">
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';

import { Autoplay, Navigation } from 'swiper';

const modules = ref([Autoplay, Navigation]);

const isOpenVideo = ref(false)

const openVideo = () => {
    isOpenVideo.value = !isOpenVideo.value
}
</script>

<style lang="scss" scoped>
.filter {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    width: 100vw;
    height: vh;
    z-index: 10;
    background: #000;
    opacity: 0;
    visibility: hidden;
    transition: .2s all;

    &.active {
        transition: .2s all;
        opacity: 0.5;
        visibility: visible;
    }
}

$white-text: #ffffff;
$raleway: 'Raleway', sans-serif;
$primary-color: #00FF91;
$light-text: #222222;



.partners {
    padding: 20px 12px;

    .swiper {
        width: 100%;
        height: 120px;
    }

    .swiper-slide {
        text-align: center;
        font-size: 18px;
        background: #fff;
        height: 100%;
        /* Center slide text vertically */
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .swiper-slide img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: contain;
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
        display: flex;
        justify-content: center;

        &::before {
            content: '';
            position: absolute;
            left: -65px;
            top: -60px;
            width: 246px;
            height: 246px;
            background-color: $primary-color;

            @media (max-width:992px) {
                width: 80px;
                height: 80px;
                left: 5px;
                top: -40px;
            }

            @media (max-width:500px) {
                width: 60px;
                height: 60px;
                left: 0px;
                top: -25px;
            }
        }

        &::after {
            content: '';
            position: absolute;
            bottom: -30px;
            right: -30px;
            width: 246px;
            height: 246px;
            background-image: url('../assets/image/cutted-square.png');

            @media (max-width:992px) {
                width: 100px;
                height: 110px;
                right: 20px;
                bottom: -15px;
                background-position: center;
                background-size: cover;
            }

            @media (max-width:500px) {
                width: 60px;
                height: 60px;
                right: 10px;
                bottom: -10px;
            }
        }

        img {
            width: 90%;
        }
    }

    &-btn {
        cursor: pointer;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;

        img {
            user-select: none;

            @media (max-width: 576px) {
                width: 50px;
                height: 50px;
            }
        }
    }

    &__item {
        border: 2px solid $primary-color;
        position: fixed;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -70%);
        padding: 10px;
        background-color: $primary-color;
        opacity: 0;
        visibility: hidden;
        transition: .3s all;
        z-index: 11;

        &.active {
            opacity: 1;
            visibility: visible;
            transition: .3s all;
            transform: translate(-50%, -50%);
        }

        video {
            width: 100% !important;
            height: 100% !important;
        }
    }
}

.whyus {
    margin-top: 100px;
    padding-bottom: 30px;
    display: flex;
    justify-content: space-between;

    @media (max-width: 650px) {
        flex-direction: column;
        row-gap: 40px;
    }

    &__left {
        width: 46%;

        @media (max-width: 650px) {
            width: 100%;
        }

        &-title {
            font-weight: 500;
            font-size: 64px;
            line-height: 67px;
            color: $light-text;

            @media (max-width: 992px) {
                font-weight: 500;
                font-size: 51px;
                line-height: 54px;
            }

            @media (max-width: 500px) {
                font-size: 38px;
            }
        }

        &-texts {
            margin-top: 36px;
            width: 100%;
            display: flex;
            flex-direction: column;
            gap: 30px;

            @media (max-width: 500px) {
                margin-top: 16px;
            }

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

        @media (max-width: 650px) {
            width: 100%;
        }

        &-title {
            font-weight: 500;
            font-size: 51px;
            line-height: 54px;
            color: $light-text;

            @media (max-width: 500px) {
                font-size: 38px;
            }

            @media (max-width: 500px) {
                margin-top: 16px;
            }
        }

        &-subtitle {
            font-weight: 400;
            font-size: 15px;
            line-height: 27px;
            color: $light-text;
            margin-top: 36px;

            @media (max-width: 500px) {
                margin-top: 16px;
            }
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

    @media (max-width: 576px) {
        padding: 20px 0px 0px 0px;
    }

    &::before {
        content: '';
        position: absolute;
        background-image: url('../assets/image/cutted-square-two.png');
        width: 246px;
        height: 246px;
        background-size: cover;
        left: -20px;
        top: -90px;

        @media (max-width: 576px) {
            width: 130px;
            height: 130px;
            top: -25px;
        }
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
            right: -36px;
            width: 100%;
            height: 100%;
            padding-top: 110px;
            margin-top: -110px;
            padding-bottom: 80px;

            @media (max-width: 1100px) {
                right: 0;
            }

            @media (max-width:850px) {
                padding-top: 60px;
                margin-top: -60px;
            }
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

    @media (max-width: 768px) {
        display: flex;
        flex-direction: column;
    }

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

        @media (max-width: 768px) {
            width: 100%;
            position: relative;
            min-height: 500px;
        }

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

        @media (max-width: 576px) {
            min-height: auto;
            padding: 30px 0px;
        }
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

        @media (max-width: 992px) {
            padding-left: 25px;

            &-title {
                font-size: 40px;
                line-height: 46px;
            }
        }

        @media (max-width: 768px) {
            width: 100%;
        }

        @media (max-width: 576px) {
            padding: 12px;
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

                @media (max-width: 576px) {
                    width: 100px;
                    height: 100px;
                }
            }
        }

        .half__content {
            padding-top: 55px;
            padding-bottom: 60px
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