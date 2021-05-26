<template>
  <section class="w-full flex justify-center">
    <div class="min-width">
      <div class="flex justify-center space-x-1">
        <a class="step is-active"></a>
      </div>
      <div class="w-full">
        <h4 class="text-left font-bold">Pertanyaan</h4>
        <p class="pt-3">
          Dalam 4 minggu terakhir, seberapa sering Anda tiba-tiba merasa lelah?
        </p>

        <SecondaryButton
          class="border text-left border-gray-400 w-full text-gray-500 mt-4"
          label="Tidak Pernah"
        />
        <SecondaryButton
          class="border text-left border-gray-400 w-full text-gray-500 mt-4"
          label="Jarang"
        />
        <SecondaryButton
          class="border text-left border-gray-400 w-full text-gray-500 mt-4"
          label="Kadang kadang"
        />
        <SecondaryButton
          class="border text-left border-gray-400 w-full text-gray-500 mt-4"
          label="Sering"
        />
        <SecondaryButton
          class="border text-left border-gray-400 w-full text-gray-500 mt-4"
          label="Selalu"
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

<style>
.step {
  border-radius: 10px;
  height: 5px;
  padding: 0;
  margin: auto 0.5%;
  background-color: rgba(43, 128, 163, 0.2);
  box-shadow: 0px 0px 3px 2px rgb(0 0 0 / 20%);
  width: 2rem;
}

.step.is-active {
  border-radius: 10px;
  background-color: #2b80a3;
  box-shadow: 0px 0px 3px 2px rgb(0 0 0 / 20%);
}

h4 {
  color: #2b80a3;
}
</style>
