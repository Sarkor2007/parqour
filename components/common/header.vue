<template>
    <div class="header__top">
        <div class="header-logo">
            <img src="../../assets/icons/logo.svg"
                alt="logo" />
        </div>
        <nav class="header__nav">
            <ul>
                <li class="header__nav-item">
                    <nuxt-link to="/">Home</nuxt-link>
                </li>
                <li class="header__nav-item">
                    <nuxt-link to="/solutions">Solutions</nuxt-link>
                </li>
                <li class="header__nav-item">
                    <nuxt-link to="/company">Company</nuxt-link>
                </li>
                <li class="header__nav-item">
                    <nuxt-link to="/contacts">Contacts</nuxt-link>
                </li>
            </ul>
        </nav>
        <div class="header__buttons">
            <button class="header__burger-btn"
                type="button"
                :class="{ open: isOpen }"
                @click="toggleMenu">
                <span class="header__burger-lines"></span>
            </button>
            <button v-if="route.path != '/'"
                class="header__buttons-btn btn-primary">Book a demo</button>
        </div>
        <div class="burger"
            :class="{ open: isOpen }">
            <div class="burger-menu">
                <ul class="burger-menu__ul">
                    <li @click="toggleMenu"
                        class="burger-menu__ul-li">
                        <nuxt-link to="/">Home</nuxt-link>
                    </li>
                    <li @click="toggleMenu"
                        class="burger-menu__ul-li">
                        <nuxt-link to="/solutions">Solutions</nuxt-link>
                    </li>
                    <li @click="toggleMenu"
                        class="burger-menu__ul-li">
                        <nuxt-link to="/company">Company</nuxt-link>
                    </li>
                    <li @click="toggleMenu"
                        class="burger-menu__ul-li">
                        <nuxt-link to="/contacts">Contacts</nuxt-link>
                    </li>
                </ul>
            </div>
            <div class="burger-bg"
                @click="toggleMenu"></div>
        </div>
    </div>
</template>

<script setup>
import { ref } from "vue";
import { useRoute } from 'vue-router'

const isOpen = ref(false);

const route = useRoute()

const toggleMenu = () => {
    isOpen.value = !isOpen.value;
    isOpen.value ? document.body.style.overflow = 'hidden' : document.body.style.overflow = 'auto';
};

</script>

<style lang="scss" scoped>
$white-text: #ffffff;
$raleway: "Raleway", sans-serif;
$primary-color: #00ff91;
$light-text: #222222;
$blue: #0d76f4;

.header {
    &__nav {
        position: absolute;
        left: 50%;
        transform: translateX(-50%);
        display: block;

        @media (max-width: 992px) {
            display: none;
        }

        ul {
            display: flex;
            align-items: center;
            gap: 56px;
        }

        &-item {
            a {
                font-family: $raleway;
                font-weight: 500;
                font-size: 16px;
                line-height: 24px;
                color: $white-text;
                transition: .3s all;

                &:hover {
                    color: $primary-color;
                    transition: .3s all;
                    text-decoration: 2px solid underline;
                }
            }
        }
    }

    &__top {
        padding: 32px 0px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        position: relative;
    }

    &__burger {
        &-btn {
            width: 47px;
            height: 47px;
            background-color: $primary-color;
            align-items: center;
            justify-content: center;
            border-radius: 4px;
            cursor: pointer;
            display: none;

            @media (max-width: 992px) {
                display: flex;
            }
        }

        &-lines {
            width: 20px;
            height: 2px;
            background-color: $blue;
            position: relative;

            &::before,
            &::after {
                content: "";
                display: block;
                width: 20px;
                height: 2px;
                background-color: $blue;
            }

            &::before {
                position: absolute;
                bottom: 8px;
            }

            &::after {
                position: absolute;
                top: 8px;
            }
        }
    }

    .burger {
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        z-index: 100;
        pointer-events: none;

        &.open {
            display: block;
            pointer-events: all;

            .burger-menu {
                transform: translateX(0);
                transition: transform .4s;
            }

            .burger-bg {
                opacity: 1;
                transition: opacity .2s;
            }
        }

        &-menu {
            position: absolute;
            left: 0px;
            top: 0;
            padding: 100px 0 80px;
            height: 100%;
            background: white;
            z-index: 1;
            transform: translateX(-100%);
            display: flex;
            flex-direction: column;
            transition: transform .4s;

            &__ul {
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 10px;
                list-style: none;
                min-width: 300px;

                &-li {
                    width: 100%;
                    display: flex;
                    justify-content: center;
                    align-items: center;

                    &:hover {
                        background-color: $blue;

                        a {
                            color: $white-text;
                        }
                    }

                    a {
                        width: 100%;
                        height: 100%;
                        font-weight: 500;
                        font-size: 16px;
                        line-height: 24px;
                        color: $light-text;
                        text-align: center;
                        padding: 10px 20px;
                    }
                }
            }
        }

        &-bg {
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            opacity: 0;
            backdrop-filter: blur(2px);
            transition: opacity .2s;
        }
    }

    &__buttons {
        display: flex;
        gap: 16px;
        align-items: center;

        &-btn {
            color: $light-text;

            @media (max-width:992px) {
                display: none;
            }
        }
    }
}</style>