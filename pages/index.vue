<template>
  <MentalTest />
</template>

<script>
export default {};
</script>

<style>
nav {
  width: 100%;
  box-shadow: 0 2px 4px -1px rgb(0 0 0 / 20%), 0 4px 5px 0 rgb(0 0 0 / 14%),
    0 1px 10px 0 rgb(0 0 0 / 12%);
}

.nav {
  min-width: 480px;
  width: 480px;
}

section {
  min-width: 480px;
  width: 480px;
}

.head::after {
  content: "";
  border-bottom: 4px solid #2b80a3;
  width: 30%;
  display: block;
  margin-top: 1rem;
}

.min-width {
  min-width: 480px;
  width: 480px;
  /* padding: 0 1rem; */
}
</style>
