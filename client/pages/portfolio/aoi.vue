<template>
    <section class="portfolio-detail">
        <div class="pf-detail-inner">
            <div class="img">
                <img src="https://i.ibb.co/6WTxHvc/aoi-content.jpg" alt="포트폴리오 메인시안">
            </div>
            <ul class="pf-info">
                <li>
                    <span>project</span>
                    <p>플로리스트 홈페이지</p>
                </li>
                <li>
                    <span>position</span>
                    <p>웹디자인 100%, 퍼블리싱 100%</p>
                </li>
                <li>
                    <span>skill</span>
                    <p>html5, css3, javascript, jquery</p>
                </li>
                <li>
                    <span>view code</span>
                    <a href="https://github.com/kimjihun-dev/floist_aoi_flower" target="_blank">github</a>
                </li>
                <li>
                    <span>view site</span>
                    <a href="https://aoiflower.netlify.app" target="_blank">demo</a>
                </li>
            </ul>
            <div class="pf-detail">
                <h4>project detail</h4>
                <p>플로리스트 아오이 플라워의 개인 홍보사이트를 제작하였습니다.<br>
                    개인의 이력 및 홍보를 위해 매번 PDF 파일로 어필을 했던 부분에 불편함을 느껴서 간단한 홍보를 위한<br>
                    홈페이지가 있다면 좋겠다고 하여 제작을 하였습니다.<br>
                    이력과 취급품목, 클래스 안내, SNS 등으로 구성하였습니다.<br>
                    PC 버전과 모바일 버전의 반응형으로 제작하였고 꽃의 이미지들은 실제로 플로리스트분이 직접 만든 작품들입니다.<br>
                    배포 및 유지보수의 편의성을 위해 VUE.JS 기반의 NUXT 프레임워크로 제작하였고,  NETLIFY 에 배포를 하였습니다.
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
            title: '플로리스트 홈페이지'
        }
    }
}
</script>

<style>
</style>
