<script setup>
import mainPhoto from "../assets/images/hero.svg";
import { themeColor } from "../data/items";

const heroHeading = "Selamat Datang di Nira Digital";
const buttonJasa = "Jasa Tugas";
const buttonTopUp = "Topup Diamond & Streaming";
const buttonUndangan = "Undangan Digital"
const buttonBuat = "Buat Aplikasi"
const buttonSC = "Source Code"
</script>

<template>
  <div class="untree_co-hero" id="home-section">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="row align-items-center">
            <div
              class="col-lg-7 ml-auto order-lg-2"
              data-aos="fade-right"
              data-aos-delay="400"
            >
              <img :src="mainPhoto" alt="Image" class="img-fluid" />
            </div>
            <div class="col-lg-5">
              <h1 class="heading" data-aos="fade-up" data-aos-delay="0">
                {{ heroHeading }}
              </h1>
              <div class="excerpt" data-aos="fade-up" data-aos-delay="100">
                <p>
                  Ini adalah landing page yang menampilkan kumpulan website yang dikelola oleh
                  <span
                    style="
                      background-color: rgba(64, 123, 255, 0.07);
                      color: #407bff;
                    "
                    >Nira Digital</span
                  >
                </p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200" class="button-container">
                <a
                  href="#jasa-section"
                  class="btn btn-primary smoothscroll"
                  :style="[
                    { background: themeColor }, { borderColor: themeColor }]"
                  >{{ buttonJasa }}</a
                >
                <a
                  href="#topup-section"
                  class="btn btn-outline-primary smoothscroll pricing"
                  :style="[{ color: themeColor }, { borderColor: themeColor }]"
                  >{{ buttonTopUp }}</a
                >
                <a
                  href="#features-section"
                  class="btn btn-primary smoothscroll"
                  :style="[
                    { background: themeColor }, { borderColor: themeColor }]"
                  >{{ buttonUndangan }}</a
                >
                <a
                  href="#pricing-section"
                  class="btn btn-outline-primary smoothscroll pricing"
                  :style="[{ color: themeColor }, { borderColor: themeColor }]"
                  >{{ buttonBuat }}</a>
                <a
                  href="#features-section"
                  class="btn btn-primary smoothscroll"
                  :style="[
                    { background: themeColor }, { borderColor: themeColor }]"
                  >{{ buttonSC }}</a
                >
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.button-container {
  display: flex;
  flex-direction: column; /* Mengatur tombol dalam kolom */
  gap: 10px; /* Jarak antar tombol */
}
.pricing:hover {
  color: #fff !important;
}
</style>
