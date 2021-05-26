<template>
  <section class="w-full flex justify-center">
    <div class="flex justify-center">
      <div class="min-width">
        <img
          class="pt-12"
          src="~/assets/mental_health.png"
          alt="mental health"
          width="420"
        />
        <div class="head text-gray-800">
          <h1 class="font-bold text-2xl">Mental Health Test</h1>
        </div>
        <p class="font-bold text-sm mt-2 text-gray-500">
          Mental Health Test membantu kamu mengetahui keyakinan dirimu dalam
          menghadapi situasi untuk berhasil mencapai hasil yang kamu inginkan.
        </p>

        <div class="w-full flex justify-center py-12">
          <PrimaryButton
            @click="clickStart"
            label="Mulai"
            class="px-16"
          />
        </div>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  props: {
    toggle: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {
    };
  },
  methods: {
    clickStart() {
      this.$emit('click', this.toggle)
    },
  },
};
</script>
