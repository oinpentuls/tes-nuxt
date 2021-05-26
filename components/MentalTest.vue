<template>
  <div>
    <nav class="flex justify-center fixed z-10 bg-white relative">
      <div class="nav">
        <img
          class="py-2"
          src="~/assets/ibunda.png"
          width="120"
          alt="logo ibunda"
        />
      </div>
    </nav>

    <FrontPage v-if="frontpage" @click="startButton" />
    <Agreement v-if="start"  @click="agreeButton" @decline="declineButton" />
    <Bridge v-if="agreement" />
    <Questionnaire v-if="agreement" />
    <Final v-if="agreement" />
    <Result v-if="agreement" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      frontpage: true,
      start: false,
      agreement: false
    };
  },
  methods: {
    startButton() {
      this.start = true
      this.frontpage = false
    },
    agreeButton() {
      this.agreement = true
      this.frontpage = false
    },
    declineButton() {
      this.agreement = false
      this.frontpage = true
    },
  },
};
</script>
