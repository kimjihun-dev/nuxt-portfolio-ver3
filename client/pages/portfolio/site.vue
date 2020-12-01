<template>
    <section class="portfolio-detail">
        <div class="pf-detail-inner">
            <div class="img">
                <img src="https://i.ibb.co/GxTmP3R/site-content02.jpg" alt="포트폴리오 메인시안">
            </div>
            <ul class="pf-info">
                <li>
                    <span>project</span>
                    <p>포트폴리오 사이트 구축</p>
                </li>
                <li>
                    <span>position</span>
                    <p>웹디자인 100%, 퍼블리싱 100%</p>
                </li>
                <li>
                    <span>skill</span>
                    <p>html5, css3, vue, nuxt</p>
                </li>
                <li>
                    <span>view code</span>
                    <a href="#!" target="_blank">github</a>
                </li>
                <li>
                    <span>view site</span>
                    <a href="#!" target="_blank">demo</a>
                </li>
            </ul>
            <div class="pf-detail">
                <h4>project detail</h4>
                <p>포트폴리오 사이트는 단순한 레이아웃 형태이지만 vue nuxt.js 프레임워크로 제작하였습니다.<br>
                기본적인 폴더구성과 컴포넌트 개념을 익혔고, 각 컴포넌트마다 스타일과 스크립트를 별도로 지정할 수 있다는 부분에서<br>
                유지보수의 편리함을 느꼈습니다. assets 동적파일, nuxt.config.js 파일을 이용한 외부 라이브러리 적용법을 익혔으며, <br>
                about, portfolio 등의 컨텐츠들을 라우팅으로 설정하는 부분도 공부하게 되었습니다. <br>
                포트폴리오 리스트들을 관리하는 코드는 아래와 같이 구현을 하였고 netlify 에 배포를 하였습니다.
                </p>
                <p>
                    <img src="~assets/images/code01.jpg" alt="">
                </p>
                <p>
                    <img src="~assets/images/code02.jpg" alt="">
                </p>
            </div>
        </div>
        <div class="back">
            <a href="/" class="backBtn">BACK</a>
        </div>
    </section>
</template>

<script>
export default {
    head () {
        return {
            title: '포트폴리오 구축'
        }
    }
}
</script>

<style>
.pf-detail p { margin-bottom: 20px; } 
.pf-detail img { width: 80%; }
@media all and (max-width: 1024px) {
    .pf-detail img { width: 100%; }
}
</style>