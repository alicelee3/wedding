<template>
  <div class="bank_area">
      <div class="title_area _english_font _big_text _green">
        Celebrate
      </div>
    <div class="_big_text _green">
      <b>마음 전해주실 곳</b>
    </div>

    

    <bank-accordion style="margin-top: 24px;padding-bottom: 5px"/>

  </div>
</template>

<script>
import BankAccordion from "@/components/BankAccordion.vue";

export default {
  name: "bank-account-area",
  components: {
    BankAccordion,
  },
  data() {
    return {
    };
  },
  mounted() {
  },
  methods: {
  }
};
</script>

<style lang="scss" scoped>

.bank_area {
  margin-top: 56px;
  padding-bottom: 56px;
  text-align: center;
  background: var(--secondary-bg-color);
}

.title_area {
  padding-top: 54px;
  line-height: 24px;
  margin-bottom: 8px;
}

.text_area {
  margin-top: 16px;
  line-height: 30px;
  letter-spacing: -0.2%;
}
</style>
