<template>
    <div class="header__top">
        <div class="header-logo">
            <img src="../../assets/icons/logo.svg"
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
</template>


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
}
</style>