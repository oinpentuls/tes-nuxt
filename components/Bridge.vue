<template>
  <section class="w-full flex justify-center">
    <div class="">
      <p class="min-width text-sm text-gray-700 text-center">
        Jawab pertanyaan berikut berdasarkan
        <strong>seberapa sering</strong> kamu mengalami situasi tersebut dalam
        kurun waktu <strong>4 minggu</strong> terakhir.
        <strong>Pilih jawaban yang paling menggambarkan diri kamu</strong>,
        <span class="text-red-600 font-bold">
          karena tidak ada jawaban yang benar dan salah
        </span>
      </p>

      <div class="flex justify-between pt-12">
        <SecondaryButton
          label="Kembali"
          class="w-auto flex-initial btn-bridge font-bold"
        />
        <PrimaryButton label="Lanjut" class="flex-initial px-12" />
      </div>
    </div>
  </section>
</template>

<style>
ol.min-width {
  list-style: decimal;
}

.btn-bridge {
  border: 1px solid #2b80a3;
  border-radius: 5px;
  color: #2b80a3;
}
</style>
