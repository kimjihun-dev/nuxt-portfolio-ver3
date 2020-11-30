<template>
    <section class="portfolio-detail">
        <div class="pf-detail-inner">
            <div class="img some-img">
                <img src="https://i.ibb.co/Bsvw5w2/some-content.jpg" alt="포트폴리오 메인시안">
            </div>
            <ul class="pf-info">
                <li>
                    <span>project</span>
                    <p>치킨집 전단지작업</p>
                </li>
                <li>
                    <span>position</span>
                    <p>편집디자인 100%</p>
                </li>
                <li>
                    <span>skill</span>
                    <p>포토샵,일러스트</p>
                </li>
                <li>
                    <span>view code</span>
                    <!-- <a href="https://github.com/kimjihun-dev/floist_aoi_flower" target="_blank">github</a> -->
                </li>
                <li>
                    <span>view site</span>
                    <!-- <a href="https://aoiflower.netlify.app" target="_blank">demo</a> -->
                </li>
            </ul>
            <div class="pf-detail">
                <h4>project detail</h4>
                <p>부산 신평동에서 영업하고 있는 닭썸 신평점 홍보용 전단지 디자인을 하였습니다.<br>
                    식욕을 돋구는 레드색상을 배경색으로 넣었으며 실제 고객들에게 제공되는<br>
                    음식들을 촬영하여 전단지내에 배치하였습니다. 해당 매장의 사장님의 의중을 최우선으로 하여 작업하였습니다.<br>
                    일러스트로 작업을 하였으며 인쇄용 A4 사이즈로 제작 후 출력작업을 진행하였습니다.
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
            title: '전단지 작업'
        }
    }
}
</script>

<style>
.some-img img { width: 100%; }
</style>
