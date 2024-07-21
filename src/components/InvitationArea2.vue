<template>
  <div class="invitation_area">
    <p class="header _big_text _green">
      <strong>"우리 결혼합니다."</strong><br />
    </p>
    <div class="desc _large_text _gray">
      데이트를 마치고 집에 돌아갈 때면<br />
      손을 놓기가 아쉬웠습니다.<br />
      아침에 눈을 떠 하루를 마칠 때까지<br />
      종일토록 서로 곁에 있고픈 저희였습니다.<br />
      그런 소망을 이루어<br />
      평생의 가약을 맺습니다.
    </div>

    <Divider3 :padding-bottom="0" padding-right="24" padding-left="24"/>

    <div class="names _small_text _gray">
      <p>{{ male.parents }}<span class="male">의 {{ male.sub }}</span><strong>{{ male.name }}</strong></p>
      <p>{{ female.parents }}<span class="male">의 {{ female.sub }}</span><strong>{{ female.name }}</strong></p>
    </div>

    <img class="invi_main_image" src="../assets/images/new/invitation/invi_img.jpg" />

  </div>
</template>

<script>

import Divider3 from "@/components/Divider3.vue";

export default {
  name: "invitation-area",
  components: {
    Divider3,
  },
  data() {
    return {
      male: {
        parents: "천관순∙김경",
        sub: "장남",
        name: "천호성"
      },
      female: {
        parents: "이동국∙조영민",
        sub: "장녀",
        name: "이미령"
      },
    };
  },
  methods: {
  },
};
</script>

<style lang="scss" scoped>
.invitation_area {
  background: var(--secondary-bg-color);
  text-align: center;
  line-height: 0;
  .header {
    padding-top: 56px;
    line-height: 28px;
  }
  .desc {
    line-height: 30px;
    padding-bottom: 36px;
  }
  .line_area {
    padding-bottom: 36px;
  }
  .line {
    width: 382px;
    border: 0.7px solid;
    color: #D7D7D7;
  }
  .names {
    text-align: right;
    line-height: 0;
    letter-spacing: 3px;
    margin-top: 24px;
    padding-right: 68px;
    .male {
      font-size: 12.5px;
      margin-left: 26px;
      margin-right: 26px;
    }
    .female {
      font-size: 12.5px;
      margin-left: 26px;
      margin-right: 43px;
    }
  }
  .names_image {
    width: 291px;
    height: 58px;
  }
  .invi_main_image {
    margin-top: 50px;
    width: 100%;
    height: auto;
  }
}
</style>
