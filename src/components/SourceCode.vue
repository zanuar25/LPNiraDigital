<script setup>
import { themeColor } from "../data/items";
const serviceSC = "Layanan Nira Digital";
const serviceSubSC = "Source Code";
const startButtonName = "Demo Web";
</script>

<template>
  <div class="untree_co-section" id="sc-section">
    <div class="container">
      <div class="text-center">
        <span
            class="caption"
            data-aos="fade-up"
            data-aos-delay="0"
            :style="[{ color: themeColor }]">
            {{ serviceSC }}
        </span>
        <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
          {{ serviceSubSC }}
        </h3>
        <p>
          Kumpulan source code yang sudah jadi, jika berminat bisa hubungi CS.
        </p>
      </div>
      <div class="row justify-content-center">
        <div class="col-lg-10">
          <div class="row justify-content-center">
            <!-- Card 1 -->
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="100" style="margin-bottom: 20px;">
              <div class="pricing">
                <div class="body" style="background-color: beige">
                  <div class="price">
                    <img src="../assets/images/ML.png" alt="Image Description">
                    <h3>Source Name 1</h3>
                  </div>
                  <p style="margin-bottom: 1px;">Fitur :</p>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>Fitur 1</li>
                    <li>Fitur 2</li>
                    <li>Fitur 3</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-outline-primary smoothscroll button"
                      :style="[{ color: themeColor }, { borderColor: themeColor }]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
            <!-- Card 2 -->
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="100" style="margin-bottom: 20px;">
              <div class="pricing">
                <div class="body" style="background-color: beige">
                  <div class="price">
                    <img src="../assets/images/ML.png" alt="Image Description">
                    <h3>Source Name 2</h3>
                  </div>
                  <p style="margin-bottom: 1px;">Fitur :</p>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>Fitur 1</li>
                    <li>Fitur 2</li>
                    <li>Fitur 3</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-outline-primary smoothscroll button"
                      :style="[{ color: themeColor }, { borderColor: themeColor }]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
            <!-- Card 3 -->
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="100" style="margin-bottom: 20px;">
              <div class="pricing">
                <div class="body" style="background-color: beige">
                  <div class="price">
                    <img src="../assets/images/ML.png" alt="Image Description">
                    <h3>Source Name 3</h3>
                  </div>
                  <p style="margin-bottom: 1px;">Fitur :</p>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>Fitur 1</li>
                    <li>Fitur 2</li>
                    <li>Fitur 3</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-outline-primary smoothscroll button"
                      :style="[{ color: themeColor }, { borderColor: themeColor }]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
            <!-- Card 4 -->
            <div class="col-lg-4" data-aos="fade-up" data-aos-delay="100" style="margin-bottom: 20px;">
              <div class="pricing">
                <div class="body" style="background-color: beige">
                  <div class="price">
                    <img src="../assets/images/ML.png" alt="Image Description">
                    <h3>Point Of Sale Toko</h3>
                  </div>
                  <p style="margin-bottom: 1px;">Fitur :</p>
                  <ul class="list-unstyled ul-check primary mb-5">
                    <li>Fitur 1</li>
                    <li>Fitur 2</li>
                    <li>Fitur 3</li>
                  </ul>
                  <p class="text-center mb-0">
                    <a
                      href="#"
                      class="btn btn-outline-primary smoothscroll button"
                      :style="[{ color: themeColor }, { borderColor: themeColor }]"
                      >{{ startButtonName }}</a
                    >
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
  .row.justify-content-center {
    display: flex;
    justify-content: center;
  }

  .col-lg-4 {
    margin-bottom: 20px; /* Ruang antar card */
  }

  .button-container {
    display: flex;
    flex-direction: column; /* Mengatur tombol dalam kolom */
    gap: 10px; /* Jarak antar tombol */
  }

  .button:hover {
    color: #fff !important;
  }

  .price img {
    max-width: 100%; /* Membuat gambar responsif */
    height: auto; /* Mengatur tinggi otomatis */
  }
</style>
