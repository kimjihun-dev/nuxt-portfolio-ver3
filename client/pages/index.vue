<template>
  <main id="index">
      <div class="pf-inner">
          <ul class="pf-list">
              <li class="item" v-for="(item, index) in pData" :key="index">
                  <div class="item-inner">
                    <nuxt-link :to="item.path">
                        <img :src="item.thum" alt="포트폴리오 썸네일">
                        <div class="overlay">
                            <div class="overlay-title">
                                <h4>{{ item.title }}</h4>
                            </div>
                        </div>
                    </nuxt-link>
                  </div>
              </li>
          </ul>
      </div>
  </main>
</template>

<script>
export default {
    data() {
        return {
            pData: [
                { path: 'portfolio/bok', title: '박물관사이트 리뉴얼', thum: 'https://i.ibb.co/Sc5vcy2/bok-thum.jpg' },
                { path: 'portfolio/site', title: '포트폴리오 사이트 구축', thum: 'https://i.ibb.co/tYh2X9Z/site-thum.jpg' },
                { path: 'portfolio/yeonje', title: '병원사이트 리뉴얼', thum: 'https://i.ibb.co/7NYnMP8/yeonje-thum.jpg' },
                { path: 'portfolio/aoi', title: '플로리스트 홍보사이트', thum: 'https://i.ibb.co/DzRbw7h/aoi-thum.jpg' },
                { path: 'portfolio/some', title: '닭썸 전단지 작업', thum: 'https://i.ibb.co/DfWP99k/ddaksum-thum.jpg' },
                { path: 'portfolio/nts', title: '지방기상청 리뉴얼', thum: 'https://i.ibb.co/Kmh3zJ9/nts-thum.jpg' },
            ]
        }
    }
}
</script>

<style>
#index { width: 85%; margin-left: 15%; background-color: #f1f1f1; position: relative; height: 100%; }
#index .pf-inner { padding: 20px; }
#index .pf-list { padding: 35px; display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 20px; }
/* #index .pf-list .item { border: 1px solid red; } */
#index .pf-list .item .item-inner { position: relative; border: 1px solid #f1f1f1; }
#index .pf-list .item .item-inner .overlay { position: absolute; background: #222; color: #ffffff; top: 0; left: 0; right: 0; bottom: 0; width: 100%; height: 100%; text-align: center; vertical-align: top; opacity: 0; transition: all 0.4s ease-in-out; }
#index .pf-list .item .item-inner .overlay-title { position: absolute; top: 50%; left: 50%;  -webkit-transform: translate(-50%, -50%); -ms-transform: translate(-50%, -50%); transform: translate(-50%, -50%); }
#index .pf-list .item .item-inner .overlay-title h4 { font-size: 16px; font-weight: normal; }
#index .pf-list .item:hover .overlay { opacity: 0.9; }

#index .pf-list .item .item-inner a { width: 100%; height: 100%; }
#index .pf-list .item .item-inner a img { width: 100%; height: 300px; }
@media all and (max-width: 1024px) {
    #index { width: 100%; margin-left: 0; }
}
</style>
