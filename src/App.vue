<script setup>
// import HelloWorld from './components/HelloWorld.vue'
// import { Dropdown, ListGroup, ListGroupItem } from 'flowbite-vue'
import NavbarComponent from './components/NavbarComponent.vue';
import HeaderComponent from "./components/HeaderComponent.vue";
import BodyComponent from "./components/BodyComponent.vue";
import FooterComponent from './components/FooterComponent.vue';
import ContactComponent from './components/ContactComponent.vue';
</script>

<script>
export default {
  data() {
    return {
      biodata: [
        ['Nama', 'M. Ridwan Nurfauzi'],
        ['TTL', 'Bandung, 3 Mei 2006'],
        ['Agama', 'Islam'],
        ['Jenis Kelamin', 'Laki-laki'],
        ['Asal Sekolah', 'SMK Assalaam bandung']
      ]
    }
  }
}
</script>

<template>
  <div>
    <NavbarComponent class="shadow-md">
      <template #title>
        <h3 class="font-semibold text-lg ms-2">
          Web Saya
        </h3>
      </template>
    </NavbarComponent>
    <HeaderComponent class="shadow-md">
      <template #title>
        <h2 class="font-bold text-3xl text-center my-7">Selamat Datang di Web Saya</h2>
      </template>
      <template #text>
        <p class="text-center my-5 drop-shadow-md">
          Ini adalah halaman utama pada Web yang saya buat.
        </p>
      </template>
      <template #body>
        <div class="text-center">
          <a href="#bio">
            <button type="button"
              class="hover:px-10 hover:shadow-lg transition-all bg-blue-600 hover:bg-blue-500 py-1 px-5 focus:ring-2 rounded text-white">
              Start
            </button>
          </a>
        </div>
      </template>
    </HeaderComponent>
    <BodyComponent v-bind:biodata="biodata"></BodyComponent>

    <ContactComponent></ContactComponent>
    
    <FooterComponent>
      <template #text1>
        Copyright &COPY; 2023
        <a href="https://www.instagram.com/kkrdwn_" class="text-blue-600 hover:underline" target="_blank">@kkrdwn_</a>
      </template>
      <template #text2>
        Made with
        <i class="bi bi-heart-fill text-red-600"></i>
      </template>
    </FooterComponent>
  </div>
</template>

<script>

</script>
