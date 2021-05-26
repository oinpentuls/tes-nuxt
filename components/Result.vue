<template>
  <section class="w-full flex justify-center">
    <div class="min-width">
      <div>
        <img class="warning" src="~/assets/warning.png" alt="warning" />
        <h1 class="text-xl font-bold">Yuk Cek Hasilnya!</h1>
        <p>Kamu sudah berhasil mengisi Test Kesehatan Online by Ibunda.id</p>
        <p>- Konseling Dengan Psikolog. Hasilnya menunjukan...</p>

        <div class="border border-gray-500 p-5 text-gray-500">
          <h4 class="text-gray-700"><strong>Oh, Kamu Membutuhkan Sedikit Bantuan!</strong></h4>
          <p class="">
            Berdasarkan hasil screening kesehatan mental, saat ini kondisimu
            tergolong kurang stabil. Kamu mungkin membutuhkan sedikit bantuan
            untuk melewati situasi ini. Coba ingat-ingat lagi, adakah hal yang
            membuat kamu merasa kurang nyaman atau mengganggumu dalam beberapa
            hari belakangan ini? Jangan ragu untuk bercerita mengenai hal
            tersebut pada teman, keluarga, atau orang yang kamu percaya ya. Kamu
            juga bisa cerita ke Bunda lewat LINE
            <a href="http://bit.ly/ibundaLINE">http://bit.ly/ibundaLINE.</a>
            Selalu ingat, kamu tidak sendirian.
          </p>
        </div>

        <SecondaryButton
          label="Download Hasil"
          class="w-full mt-6 flex-initial text-center btn-bridge font-bold"
        />
        <div class="flex justify-between mt-6 ">
          <PrimaryButton class="px-12" label="Cari Bantuan" />
          <SecondaryButton
            label="Kembali ke Beranda"
            class="w-auto flex-initial btn-bridge font-bold"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.warning {
  background: url("assets/bg-result.png");
  background-position: center;
  background-repeat: no-repeat;
  background-size: contain;
}
</style>
