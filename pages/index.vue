<template>
  <div>
    <nav class="flex justify-center fixed z-10 bg-white">
      <div class="nav">
        <img
          class="py-2"
          src="~/assets/ibunda.png"
          width="120"
          alt="logo ibunda"
        />
      </div>
    </nav>
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
            <button class="bg-blue-100 py-4 px-20 btn-start rounded">
              Mulai
            </button>
          </div>
        </div>
      </div>
    </section>
  </div>
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
  padding: 0 1rem;
}

.btn-start {
  background: #2b80a3;
  color: white;
  text-align: center;
  font-weight: bold;
}
</style>
