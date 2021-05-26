<template>
  <section
    class="w-full flex justify-center absolute pt-6"
    @agree="$emit('agree', toggle)"
    @decline="$emit('agree', toggle)"
  >
    <div class="">
      <ol class="min-width text-gray-700">
        <li>
          Test ini TIDAK ditujukan untuk mendiagnosis gangguan psikologis, namun
          untuk membantu mengenali gambaran dirimu saat ini
        </li>
        <li>
          Apabila kamu mengalami gejala yang mengganggu, segeralah berkonsultasi
          ke psikolog/psikiater untuk mendapatkan penanganan yang tepat.
        </li>
      </ol>

      <div class="pt-6">
        <SecondaryButton
          @click="clickStart"
          class="w-full text-left border border-gray-400 text-gray-600"
          label="Ya, saya setuju"
        />
        <SecondaryButton
          @click="clickStart"
          class="w-full text-left mt-6 border border-gray-400 text-gray-600"
          label="Tidak, saya tidak setuju"
        />
      </div>
      <div class="w-full flex justify-center pt-6" v-if="toggle">
        <PrimaryButton
          @click="clickStart"
          label="Lanjut"
          class="w-auto text-center px-24"
        />
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
    return {};
  },
  methods: {
    clickStart() {
      this.$emit("click", this.toggle);
      this.$emit("decline", this.toggle);
    },
  },
};
</script>
<style>
ol.min-width {
  list-style: decimal;
}
</style>
