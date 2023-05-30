<template>
    <div class="page">

        <header class="header">
            <div class="container">
                <CommonHeader></CommonHeader>
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

        <SiteContent></SiteContent>

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
                                <h3> {{ item.header }} </h3>
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


        <CommonFooter></CommonFooter>
    </div>
</template>

<script setup lang="ts">

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



.header {
    background: #0D76F4;
    background-image: url('../assets/image/main-bg.png');
    background-position: right center;
    background-size: contain;
    background-repeat: no-repeat;
    min-height: 850px;

    @media (max-width: 640px) {
        min-height: 950px;
    }

    @media (max-width: 576px) {
        min-height: 870px;
    }
    @media (max-width: 360px) {
        min-height: 920px;
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

            @media (max-width: 510px) {
                font-size: 40px;
                line-height: 50px;
            }
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

        @media (max-width: 640px) {
            flex-direction: column;
            row-gap: 20px;
            align-items: flex-start;
        }

        @media (max-width: 576px) {
            row-gap: 30px;
        }


        &-item {
            display: flex;
            align-items: center;
            gap: 16px;

            @media (max-width: 640px) {
                gap: 50px;
            }

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
    z-index: 2;
    margin-bottom: 300px;

    img {
        padding: 0px 12px;
        left: 0;
        width: 100%;
        border-radius: 24px;
        position: absolute;
        transform: translateY(-50%);
    }

    @media (max-width: 992px) {
        img {
            height: 400px;
            object-fit: cover;
        }
    }

    @media (max-width: 768px) {
        img {
            padding: 0px;
            transform: translateY(-30%);
        }
    }


    @media (max-width: 576px) {
        margin-top: 30px;
        height: 400px;
        margin-bottom: 30px;

        img {
            height: 100%;
            position: static;
            transform: translateY(-0%);
            object-position: right;
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

        @media (max-width: 992px) {
            width: 80px;
            height: 80px;
            bottom: 0px;
            right: -10px;
        }
    }

    .answers-wrapper {
        padding: 90px 12px 85px;
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

                    @media (max-width: 576px) {
                        font-size: 18px;
                        line-height: 22px;
                    }
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

        @media (max-width: 992px) {
            width: 100%;
        }
    }

    &-title {
        font-weight: 500;
        font-size: 64px;
        line-height: 67px;
        color: $white-text;

        @media (max-width: 576px) {
            font-size: 36px;
            line-height: 40px;
        }
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

        @media (max-width: 576px) {
            padding: 0px;
        }

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
</style>


<style lang="scss">
$primary-color: #00FF91;

.btn-primary {
    background: $primary-color;
    border-radius: 4px;
    padding: 11px 24px 12px;
    font-weight: 500;
    font-size: 16px;
    line-height: 24px;
    text-align: center;
    cursor: pointer;
    transition: .3s all;

    &:hover {
        transition: .3s all;
        background-color: #aeffdc;
    }
}
</style>