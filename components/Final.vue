<template>
  <section class="w-full flex justify-center">
    <div class="min-width">
      <div class="flex justify-center space-x-1">
        <a class="step is-active"></a>
      </div>
      <div class="w-full">
        <h4 class="text-left">Email</h4>
        <p class="pt-3 text-gray-500 text-sm font-bold">Isi dengan email aktif yang kamu gunakan</p>

        <input
          placeholder="Example: hallo@ibunda.id"
          class="border border-gray-400 w-full text-gray-500 mt-4 h-12 pl-5 rounded-md"
        />

        <div class="flex mt-6 items-center justify-between">
          <SecondaryButton
            label="Kembali"
            class="w-auto flex-initial btn-bridge font-bold"
          />
          <p class="text-sm text-gray-400">1 dari 11</p>
          <PrimaryButton label="Lanjut" class="px-8" />
        </div>
      </div>
    </div>
  </section>
</template>
