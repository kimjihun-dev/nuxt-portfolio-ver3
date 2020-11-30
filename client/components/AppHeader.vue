<template>
    <header id="header">
        <h1 class="logo">
            <nuxt-link to="/">portfolio</nuxt-link>
        </h1>
        <nav id="nav">
            <ul class="gnb">
                <li v-for="(item, index) in navLinks" :key="index">
                    <nuxt-link :to="item.path" exact>{{ item.title }}</nuxt-link>
                </li>
            </ul>
            <ul class="icons">
                <li>
                    <a href="https://github.com/kimjihun-dev" target="_blank" title="깃허브">
                        <img src="~assets/images/github.png" alt="github icon">
                    </a>
                </li>
                <li>
                    <a href="mailto:zodlab@kakao.com" target="_blank" title="메일주소">
                        <img src="~assets/images/mail.png" alt="mail icon">
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            navLinks: [
                { path: '/', title: 'Home' },
                { path: '/about', title: 'About' },
            ]
        }
    }
}
</script>

<style>
#header { background-color: #fff; width: 15%; height: 100%; position: fixed; top: 0; left: 0; }
#header { text-align: center; padding-top: 100px; }
/* logo */
#header .logo { margin-bottom: 100px; display: flex; justify-content: center;}
#header .logo a { display: block; text-indent: -9999px; width: 143px; height: 21px; background: url('~assets/images/logo.png') no-repeat; background-size: 100%; }
/* gnb */
#nav .gnb { margin-bottom: 100px; }
#nav .gnb li { margin-bottom: 35px; }
#nav .gnb li a { text-decoration: none; color: #666666; font-size: 15px; letter-spacing: -1px; }
#nav .gnb li a.nuxt-link-active { color: #cc0000; }
/* icons */
#nav .icons li { display: inline-block; vertical-align: middle; }
#nav .icons li:nth-child(1) { margin-right: 10px; }

/* moblie ~ 1024px */
@media all and (max-width: 1024px) {
    #header { position: relative; width: 100%; height: 70px; padding-top: 0; text-align: initial; display: flex; justify-content: space-between; padding: 0 5%; line-height: 70px; }
    #header .logo { display: block; padding-top: 28px; }
    #header .logo a { width: 123px; height: 21px; background: url('~assets/images/logo.png') no-repeat; background-size: 100%; }
    #nav { display: flex; }
    #nav .gnb { display: flex; margin-right: 35px; width: 100px; justify-content: space-between; }
    #nav .icons { padding-top: 5px; display: flex; justify-content: space-between; width: 50px; }
    #nav .icons li:nth-child(1) { margin: 0; }
}
</style>