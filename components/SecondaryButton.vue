<template>
  <button :class="`btn-agreement ${className}`" @click="toggleValue">
    {{ label }}
  </button>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: "",
    },
    className: {
      type: String,
      default: "",
    },
    toggle: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {};
  },
  methods: {
    toggleValue() {
      this.$emit("click", this.toggle);
    },
  },
};
</script>

<style>
.btn-agreement {
  transition: ease-in 0.1s;
  padding: 0.8rem 1.7rem;
  /* display: block; */
  /* border: 1px solid; */
  border-radius: 5px;
  /* text-align: left; */
}

.btn-agreement:hover {
  background: #2b80a3;
  color: white;
}
</style>
