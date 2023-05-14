<template>
    <div class="page">
        <header class="header">
            <div class="container">
                <CommonHeader :headerBtn="headerBtn"></CommonHeader>
                <main class="header__main">
                    <h3 class="header__main-subtitle">Contacts</h3>
                    <h1 class="header__main-title">We’re a distributed team</h1>
                    <p class="header__main-text">We have offices and teams all around the world.</p>
                </main>
                <div class="header__map">
                    <img width='100%'
                        src="../assets/image/locations.png"
                        alt="map">
                    <div class="header__locations">
                        <div class="header__locations-item">
                            <div class="header__locations-cord us">
                                <span></span>

                            </div>
                            <div class="header__locations-clue us">
                                <img src="../assets/image/flags/US.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">US</h3>
                                <p class="header__locations-text">2112 Chestnut St, Suite 112, Alhambra, CA 91803</p>
                                <h4 class="header__locations-phone"> +1 516 468 1202
                                </h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">
                            <div class="header__locations-cord uz">
                                <span></span>
                            </div>
                            <div class="header__locations-clue uz">
                                <img src="../assets/image/flags/UZ.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">Uzbekistan</h3>
                                <p class="header__locations-text">Ahmad Donish St. 12, District 21A,Tashkent 10018</p>
                                <h4 class="header__locations-phone"> +998-917-966006</h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">

                            <div class="header__locations-cord kz">
                                <span></span>
                            </div>
                            <div class="header__locations-clue kz">
                                <img src="../assets/image/flags/KZ.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">Kazakhstan</h3>
                                <p class="header__locations-text">Shevchenko St. 144, Almaty</p>
                                <h4 class="header__locations-phone">+7 771 553 11 85
                                </h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">

                            <div class="header__locations-cord uk">
                                <span></span>
                            </div>
                            <div class="header__locations-clue uk">
                                <img src="../assets/image/flags/GB.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">UK</h3>
                                <p class="header__locations-text">239 Gable House Regents Park Road London,N3 3LF</p>
                                <h4 class="header__locations-phone">+447957020077</h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">
                            <div class="header__locations-cord ch">
                                <span></span>
                            </div>
                            <div class="header__locations-clue ch">
                                <img src="../assets/image/flags/CH.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">Switzerland</h3>
                                <p class="header__locations-text">Grafenaustrasse 15 Zug 6300</p>
                                <h4 class="header__locations-phone">+41 79 587 38 91</h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">

                            <div class="header__locations-cord ae">
                                <span></span>
                            </div>
                            <div class="header__locations-clue ae">
                                <img src="../assets/image/flags/AE.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">UAE</h3>
                                <p class="header__locations-text">247-0 Alsuaidi Al Mararr, Dubai</p>
                                <h4 class="header__locations-phone">+971 50 105 88 72</h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">
                            <div class="header__locations-cord vn">
                                <span></span>
                            </div>
                            <div class="header__locations-clue vn">
                                <img src="../assets/image/flags/VN.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">Vietnam</h3>
                                <p class="header__locations-text">V11- B09, Khu đô thị mới An Hưng, Phường La Khê, Quận Hà
                                    Đông, Thành Phố Hà Nội, Việt Nam</p>
                                <h4 class="header__locations-phone">+84 888 1616 55</h4>
                                <div class="triangle"></div>
                            </div>
                        </div>
                        <div class="header__locations-item">
                            <div class="header__locations-cord id">
                                <span></span>
                            </div>
                            <div class="header__locations-clue id">
                                <img src="../assets/image/flags/ID.png"
                                    alt="uz flag">
                                <h3 class="header__locations-name">Indonesia</h3>
                                <p class="header__locations-text">PT. PARQOUR PARKING TECHNOLOGIES GoWork Plaza Indonesia,
                                    5th Level Unit E021AB, Jl. MH Thamrin Kav. 28-30, Jakarta 10350</p>
                                <div class="triangle"></div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <div class="contacts">
            <div class="container">
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/US.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">US</h3>
                    <h4 class="contacts__item-phone">+1 516 468 1202</h4>
                    <p class="contacts__item-text">2112 Chestnut St, Suite 112,
                        Alhambra, CA 91803</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/CH.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">Switzerland</h3>
                    <h4 class="contacts__item-phone">+41 79 587 38 91</h4>
                    <p class="contacts__item-text">Grafenaustrasse 15
                        Zug 6300</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/GB.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">UK</h3>
                    <h4 class="contacts__item-phone">+447957020077</h4>
                    <p class="contacts__item-text">239 Gable House
                        Regents Park Road
                        London,N3 3LF</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/AE.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">UAE</h3>
                    <h4 class="contacts__item-phone">+971 50 105 88 72</h4>
                    <p class="contacts__item-text">247-0 Alsuaidi
                        Al Mararr, Dubai</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/VN.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">Vietnam</h3>
                    <h4 class="contacts__item-phone">+84 888 1616 55</h4>
                    <p class="contacts__item-text">V11- B09, Khu đô thị mới An
                        Hưng, Phường La Khê,
                        Quận Hà Đông,
                        Thành Phố Hà Nội, Việt Nam</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/ID.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">Indonesia</h3>
                    <p class="contacts__item-text">PT. PARQOUR PARKING
                        TECHNOLOGIES
                        GoWork Plaza Indonesia,
                        5th Level Unit E021AB,
                        Jl. MH Thamrin Kav. 28-30,
                        Jakarta 10350</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/KZ.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">Kazakhstan</h3>
                    <h4 class="contacts__item-phone">+7 771 553 11 85</h4>
                    <p class="contacts__item-text">Shevchenko St. 144,
                        Almaty</p>
                </div>
                <div class="contacts__item">
                    <div class="contacts__item-flag">
                        <img src="../assets/image/flags/UZ.png"
                            alt="usa flag">
                    </div>
                    <h3 class="contacts__item-name">Uzbekistan</h3>
                    <h4 class="contacts__item-phone">+998 917 966006</h4>
                    <p class="contacts__item-text">Ahmad Donish St. 12,
                        District 21A,
                        Tashkent 10018</p>
                </div>
            </div>
        </div>

        <CommonFooter></CommonFooter>

    </div>
</template>

<script setup lang="ts">
let headerBtn = true;
</script>

<style lang="scss" scoped>
$white-text: #ffffff;
$raleway: 'Raleway', sans-serif;
$primary-color: #00FF91;
$light-text: #222222;



.header {
    background: #0D76F4;
    min-height: 300px;

    &__main {
        padding: 60px 0px 70px;
        display: flex;
        flex-direction: column;
        align-items: center;

        &-title {
            font-family: $raleway;
            font-weight: 700;
            font-size: 48px;
            line-height: 56px;
            text-align: center;
            color: $white-text;
            margin-top: 12px;

            @media (max-width: 576px) {
                font-size: 36px;
                line-height: 40px;
            }
        }

        &-subtitle {
            font-family: $raleway;
            font-weight: 600;
            font-size: 16px;
            line-height: 24px;
            text-align: center;
            color: #00FF91;
        }

        &-text {
            font-family: $raleway;
            font-weight: 400;
            font-size: 20px;
            line-height: 28px;
            text-align: center;
            color: $white-text;
            opacity: 0.8;
            margin-top: 24px;
        }
    }

    &__map {
        width: 100%;
        max-width: 1024px;
        margin: auto;
        display: flex;
        justify-content: center;
        padding-bottom: 80px;
        position: relative;

        @media (max-width:992px) {
            display: none;
        }
    }

    &__locations {
        position: absolute;
        width: 100%;
        height: 100%;

        .us {
            left: 18%;
            top: 24%
        }

        .uz {
            left: 69%;
            top: 30%;
        }

        .kz {
            left: 71%;
            top: 23%;

            .triangle {

                &::after {
                    bottom: -34px;
                }
            }
        }

        .uk {
            left: 47%;
            top: 24%;
        }

        .ch {
            left: 53%;
            top: 29%;

            .triangle {

                &::after {
                    bottom: -34px;
                }
            }
        }

        .ae {
            left: 61%;
            top: 43%;

            .triangle {

                &::after {
                    bottom: -34px;
                }
            }
        }

        .vn {
            left: 76%;
            top: 47%;
        }

        .id {
            left: 78%;
            top: 53%;
        }

        &-cord {
            position: absolute;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            z-index: 1;

            span {
                position: absolute;
                z-index: 2;
                background: $primary-color;
                border-radius: 28px;
                width: 8px;
                height: 8px;
                box-shadow: 0px 0px 7px 4px $primary-color;
            }

            &:hover {
                &+.header__locations-clue {
                    opacity: 1;
                    visibility: visible;
                    transition: .3s;
                }
            }
        }

        &-clue {
            z-index: 999;
            transition: .3s;
            transition-delay: .1s;
            opacity: 0;
            visibility: hidden;
            transform: translate(-47%, -115%);
            position: absolute;
            width: 230px;
            min-height: 140px;
            background-color: $white-text;
            border-radius: 8px;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 12px 16px;

            img {
                width: 20px;
                height: 20px;
                object-fit: cover;
            }

            .triangle {
                width: 100%;
                position: relative;

                &::after {
                    content: '';
                    position: absolute;
                    left: 50%;
                    transform: translateX(-50%);
                    bottom: -18px;
                    border-top: solid 8px white;
                    border-left: solid 8px transparent;
                    border-right: solid 8px transparent;
                }
            }
        }

        &-name {
            font-weight: 600;
            font-size: 12px;
            line-height: 18px;
            text-align: center;
            color: $light-text;
            margin-top: 8px;
        }

        &-text {
            font-weight: 400;
            font-size: 12px;
            line-height: 18px;
            text-align: center;
            color: #475467;
            margin-top: 4px;
        }

        &-phone {
            font-weight: 400;
            font-size: 12px;
            line-height: 18px;
            text-align: center;
            color: #0D76F4;
            margin-top: 16px;
        }
    }
}

.contacts {
    padding: 96px 0px 50px;

    .container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 32px;

        @media (max-width: 992px) {
            grid-template-columns: repeat(3, 1fr);
        }

        @media (max-width: 992px) {
            grid-template-columns: repeat(2, 1fr);
        }

        @media (max-width: 576px) {
            grid-template-columns: 1fr;
        }
    }

    &__item {
        background: #F9FAFB;
        border-radius: 16px;
        padding: 44px 30px;
        min-height: 230px;

        position: relative;

        &-flag {
            position: absolute;
            transform: translate(-50%, -50%);
            left: 50%;
            top: 0;
            background: #EBF4FF;
            border: 8px solid #F5F9FF;
            border-radius: 28px;
            width: 48px;
            height: 48px;
            display: flex;
            justify-content: center;
            align-items: center;

            img {
                width: 24px;
                height: 24px;
                object-fit: cover;
            }
        }

        &-name {
            font-weight: 600;
            font-size: 20px;
            line-height: 30px;
            text-align: center;
            color: #101828;
        }

        &-phone {
            font-weight: 400;
            font-size: 16px;
            line-height: 24px;
            text-align: center;
            color: #475467;
            margin-top: 8px;
        }

        &-text {
            margin-top: 20px;
            font-weight: 600;
            font-size: 16px;
            line-height: 24px;
            text-align: center;
            color: #157FFF;
            text-align: center;
        }
    }
}
</style>