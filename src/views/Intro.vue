<template>
  <div class="font-sans min-h-screen">
    <div class="flex flex-row justify-center">
      <img class="h-6 mt-5 mb-10 lg:my-6 object-contain" src="../assets/logo.png" alt="">
    </div>
    <div class="flex flex-col lg:flex-row w-full pb-10">
      <div class="flex flex-col w-11/12 lg:w-6/12 px-4 md:px-10 lg:pl-32 mx-auto">
        <img class="object-contain w-4/12 lg:w-5/12 mx-auto lg:ml-0 mb-4" src="../assets/section-1.png" alt="">
        <h1 class="text-3xl md:text-3xl text-gray-800 text-center lg:text-left font-sans font-semibold">
            Selamat datang di halaman Tes Kesehatan Mental 
        </h1>
        <p class="w-full md:w-10/12 lg:w-full mx-auto pt-3 text-gray-700 text-base text-md sm:text-lg mb-8 text-center lg:text-left slide-in-bottom-subtitle leading-relaxed">
            Anda akan diminta untuk membaca pernyatan yang tertulis di tes ini. Silahkan pilih angka yang paling mewakili kondisi Anda
        </p>
        <div class="hidden lg:flex flex-row">
          <router-link to="/test">
            <v-button class="mx-auto py-3 px-10" msg="Mulai Tes"></v-button>
          </router-link>
        </div>
      </div>
      <div class="mt-10 lg:ml-40 w-full lg:w-6/12 lg:rounded-r-none lg:rounded-l-lg" style="background: #10CBE1;">     
        <div class="lg:pl-16 mt-10 text-white font-semibold">
          <p class="text-3xl lg:text-2xl pb-4 text-center lg:text-left">Skala Jawaban</p>
          <table class="table-auto mx-auto lg:ml-0">
              <thead>
                <tr class="border-b">
                  <th class="px-4 py-2 text-center">Nilai</th>
                  <th class="px-4 py-2 text-left">Keterangan</th>
                </tr>
              </thead>
              <tbody>
                <tr class="border-b">
                  <td class="px-4 py-2 text-center">0</td>
                  <td class="px-4 py-2 text-left">Tidak terjadi pada saya sama sekali</td>
                </tr>
                <tr class="border-b">
                  <td class="px-4 py-2 text-center">1</td>
                  <td class="px-4 py-2 text-left">Jarang terjadi pada saya</td>
                </tr>
                <tr class="border-b">
                  <td class="px-4 py-2 text-center">2</td>
                  <td class="px-4 py-2 text-left">Kadang-kadang terjadi pada saya</td>
                </tr>
                <tr class="border-b">
                  <td class="px-4 py-2 text-center">3</td>
                  <td class="px-4 py-2 text-left">Sering terjadi pada saya</td>
                </tr>
              </tbody>
            </table>
        </div>
        <div class="hidden lg:block relative w-7/12 xl:w-5/12 -ml-20 my-6 rounded-lg bg-white shadow-xl border-2 border-gray-100">
          <p class="absolute border w-10/12 border-gray-100" style="top:50%"></p>
          <div class="flex py-1 flex-col w-full">
            <table class="table-auto mx-auto">
              <thead>
                <tr>
                  <th class="px-5 py-3">0</th>
                  <th class="px-5 py-3">1</th>
                  <th class="px-5 py-3">2</th>
                  <th class="px-5 py-3">3</th>
                </tr>
              </thead>
              <tbody>
                <tr>
                  <td class="px-5 py-3">
                    <label class="inline-flex items-center">
                      <input type="radio" class="form-radio" name="radio" value="0" checked>
                    </label>
                  </td>
                  <td class="px-5 py-3">
                    <label class="inline-flex items-center">
                      <input type="radio" class="form-radio" name="radio" value="1">
                    </label>
                  </td>
                  <td class="px-5 py-3">
                    <label class="inline-flex items-center">
                      <input type="radio" class="form-radio" name="radio" value="2">
                    </label>
                  </td>
                  <td class="px-5 py-3">
                    <label class="inline-flex items-center">
                      <input type="radio" class="form-radio" name="radio" value="3">
                    </label>
                  </td>
                </tr>
              </tbody>
            </table>
          </div>
        </div>
        <div class="flex lg:hidden flex-col w-6/12 sm:w-3/12 mx-auto mt-20 mb-10">
          <router-link to="/test">
            <v-button class="mx-auto py-3 px-3 rounded-lg" msg="MULAI TES"></v-button>
          </router-link>
          <router-link to="/" class="mx-auto text-white text-sm mt-3" style="text-decoration:underline!important;">Kembali</router-link>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Button from '@/components/Button.vue'

export default {
  name: 'test',
  components: {
    'v-button' : Button,
  }
}
</script>

<style>

</style>