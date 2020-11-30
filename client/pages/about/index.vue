<template>
    <section class="about">
        <div class="about-inner">
            <div class="about-intro">
                <div class="about-img">
                    <img src="~assets/images/inro-kjh.png" alt="프로필 사진">
                </div>
                <div class="introTxt">
                    <span>Kim ji Hun</span>
                    <p>
                        항상 노력하는 인재 김지훈입니다. 포트폴리오 사이트를 클릭해 주셔서 정말 감사드립니다.<br>
                        30대 후반의 나이에 많지 않은 IT 실무경력으로 회사측에서 부담을 가질 수 있겠다는 생각을 가지고 있습니다.<br>
                        그럼에도 꿈은 접을 수 없어 이렇게 도전을 하고 있습니다. 저의 꿈은 60살을 넘어 70, 80살이 되어서도<br>
                        프로그래밍을 하는 것입니다.아무것도 없는 흰색 백지, 무의 상태에서 코드를 통해 무언가를 나타내는 성취감을 한번 느끼고 나니 <br>
                        굉장히 즐겁다 라는 생각을 가지게 되었습니다. <br>
                        문제점이 생길 때 구글링 또는 다양한 경로를 통해 검색하고 해결했을때의 기분도 너무 좋았습니다.<br>
                        이런 점 때문에 이 분야에 대해 전직을 준비하게 되었습니다.<br>
                    </p>
                    <p>좋은 기회가 있다면 제가 속한 조직을 위해 한 사람 몫을 할 수 있도록 최선을 다하도록 노력하겠습니다.</p>
                </div>
            </div>
            <div class="skills">
                <!-- develoment -->
                <div class="develoment">
                    <div class="develTitle">Develoment</div>
                    <div class="develList">
                        <ul>
                            <li>Html</li>
                            <li>Css</li>
                            <li>Javscript</li>
                            <li>jQuery</li>
                            <li>Vue</li>
                            <li>Python</li>
                            <li>Django</li>
                        </ul>
                    </div>
                </div>
                <!-- design -->
                <div class="design">
                    <div class="designTitle">Design Tool</div>
                    <div class="designList">
                        <ul>
                            <li>Photoshtop</li>
                            <li>Illustrator</li>
                            <li>Figma</li>
                            <li>Zeplin</li>
                            <li>Premier Pro</li>
                        </ul>
                    </div>
                </div>
                <!-- contact -->
                <div class="contact">
                    <div class="contactTitle">Contact</div>
                    <div class="contactList">
                        <ul>
                            <li>010.2697.4836</li>
                            <li>zodlab@kakao.com</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    head () {
        return {
            title: 'about'
        }
    }
}
</script>

<style>
.about { width: 85%; background: #f1f1f1; margin-left: 15%; position: relative; height: 100vh; padding: 35px; }
.about-inner { background-color: #fff; width: 100%; height: 100%; padding: 35px; }
.about-intro { display: flex; justify-content: center; }
.about-intro .introTxt { padding: 10px; margin-left: 25px; }
.about-intro .introTxt span { display: block; margin-bottom: 25px; letter-spacing: -1px; }
.about-intro .introTxt p { font-size: 16px; letter-spacing: -1px; color: #444; line-height: 1.6; }

.skills { width: 80%; margin: 0 auto; border-top: 1px solid #ddd; margin-top: 20px; padding-top: 40px; }
.develoment, .design, .contact { display: flex; margin-bottom: 45px; }
.develTitle, .designTitle, .contactTitle { font-size: 18px; font-weight: 700; color: #ef7777; width: 130px; margin-right: 20px; }
.develList ul, .designList ul, .contactList ul { display: flex; }
.develList ul li, .designList ul li, .contactList ul li { font-size: 14px; color: #444; margin-right: 35px; background-color: #f1f1f1; padding: 10px; border-radius: 5px; }
.develList ul li:hover, .designList ul li:hover, .contactList ul li:hover { opacity: 0.7; }


@media all and (max-width: 1024px) {
    .about { width: 100%; height: 100%; margin-left: 0%; }
    .about-intro { display: flex; flex-flow: column wrap; }
    .about-img { display: none; }
    .introTxt { margin-left: 0px !important; padding-left: 0px; }
    .skills { width: 100%; }
    .develoment, .design, .contact { display: flex; flex-flow: column wrap; width: 100%; }
    .develTitle, .designTitle, .contactTitle { margin-bottom: 20px; }
    .develList ul, .designList ul, .contactList ul { width: 100%; flex-flow: row wrap; }
    .develList ul li, .designList ul li, .contactList ul li { margin-right: 0px; margin-bottom: 10px; margin-right: 10px;}
}
</style>