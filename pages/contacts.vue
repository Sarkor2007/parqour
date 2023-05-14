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
                        <img src="../assets/image/flags/US.png"
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
    background-image: url('../assets/image/main-bg.png');
    background-position: right center;
    background-size: contain;
    background-repeat: no-repeat;
    min-height: 660px;

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
}

.contacts {
    padding: 96px 0px 50px;

    .container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        gap: 32px;
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