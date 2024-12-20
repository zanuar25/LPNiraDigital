<script setup>
import ML from "../assets/images/ML.png";
import GEN from "../assets/images/GENSHIN.png"; 
import VAL from "../assets/images/VAL.png"; 
import FF from "../assets/images/FF.png";
import PUBG from "../assets/images/PUBG.png";
const games = [
  { src: ML, text: "Mobile Legends", subtitle: "Moonton", link: "https://link1.com" },
  { src: GEN, text: "Genshin Impact", subtitle: "HoYoverse", link: "https://link2.com" },
  { src: VAL, text: "Valorant", subtitle: "Riot Games", link: "https://link3.com" },
  { src: FF, text: "Free Fire", subtitle: "Garena", link: "https://link4.com" },
  { src: PUBG, text: "PUBG Mobile", subtitle: "Tencent Game", link: "https://link4.com" },
];

import NET from "../assets/images/NET.png";
import YT from "../assets/images/YT.png"; 
import VIU from "../assets/images/VIU.png"; 
import PV from "../assets/images/PV.png"; 
import GC from "../assets/images/GC.png"; 
import VP from "../assets/images/VP.png";
const images = [
  { src: NET, text: "Netflix", link: "https://link1.com" },
  { src: YT, text: "Youtube Premium", link: "https://link2.com" },
  { src: VIU, text: "VIU", link: "https://link3.com" },
  { src: PV, text: "Prime Video", link: "https://link4.com" },
  { src: GC, text: "Get Contact Premium", link: "https://link5.com" },
  { src: VP, text: "Vidio Premier", link: "https://link6.com" },
];

const serviceTopUp = "Layanan Nira Digital";
const serviceSubTopUp = "TopUp Diamond";

const serviceDigital = "Layanan Nira Digital";
const serviceSubDigital = "Akun Premium Streaming";

const buttonWeb = "Website";
const buttonHub = "Hubungi Kami Sekarang"


</script>

<template>
  <div class="untree_co-section bg-light" id="topup-section">
    <div class="container">
      <div class="text-center">
        <span
            class="caption"
            data-aos="fade-up"
            data-aos-delay="0"
            :style="[{ color: themeColor }]">
            {{ serviceTopUp }}
        </span>
        <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
          {{ serviceSubTopUp }}
        </h3>
        <p>
          Penyedia topup diamond dan game terpercaya, aman, dan selalu mengutamakan kepuasan pelanggan.
        </p>
      </div>
      <div class="col-lg-12" data-aos="fade-up" data-aos-delay="400" style="display: flex; justify-content: center; gap: 10px;">
        <a v-for="(image, index) in games" :key="index" :href="image.link" class="btn-video" data-fancybox style="position: relative;">
            <div class="image-frame">
                <img :src="image.src" alt="Image" class="img-fluid img-shadow" style="width: 200px; height: auto;" />
                <div class="image-text-container">
                    <h4 class="image-title">{{ image.text }}</h4>
                    <p class="image-subtitle">{{ image.subtitle }}</p>
                </div>
            </div>
        </a>
      </div>

      <div class="text-center" style="margin-top: 60px;">
        <span
            class="caption"
            data-aos="fade-up"
            data-aos-delay="0"
            :style="[{ color: themeColor }]">
            {{ serviceDigital }}
        </span>
        <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
          {{ serviceSubDigital }}
        </h3>
        <p>
          Penyedia akun premium streaming terpercaya dan amanah, memberikan akses tanpa batas dengan kualitas terbaik dan layanan yang bisa diandalkan.
        </p>
      </div>
      <div class="col-lg-12" data-aos="fade-up" data-aos-delay="400" style="display: flex; justify-content: center; gap: 10px;">
        <a v-for="(image, index) in images" :key="index" :href="image.link" class="btn-video" data-fancybox style="position: relative;">
          <div class="image-frame">
              <img :src="image.src" alt="Image" class="img-fluid img-shadow" style="width: 200px; height: auto;" />
              <div class="image-text-container">
                <h4 class="image-title">{{ image.text }}</h4>
              </div>
          </div>
        </a>
      </div>

      <div class="text-center" style="margin-top: 60px;">
        <div style="display: flex; justify-content: center; gap: 10px;">
            <a
                href="https://topup.niradigital.my.id/"
                class="btn btn-primary smoothscroll"
                v-bind:style="{ background: themeColor, borderColor: themeColor }"
                target="_blank"
            >
                {{ buttonWeb }}
            </a>
            <a
                href="https://wa.me/1234567890" 
                class="btn btn-primary smoothscroll"
                v-bind:style="{ background: themeColor, borderColor: themeColor }"
                target="_blank"
            >
                {{ buttonHub }}
            </a>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.image-title {
    color: white;
}

.image-frame {
    position: relative;
    overflow: hidden;
    border: 2px solid #ccc; /* Ganti dengan warna bingkai yang diinginkan */
    border-radius: 8px; /* Membuat sudut bingkai melengkung */
    transition: transform 0.3s ease; /* Efek transisi saat hover */
}

.image-frame:hover {
    transform: scale(1.05); /* Membesarkan bingkai saat hover */
}

.image-text-container {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    background: rgba(0, 0, 0, 0.7); /* Latar belakang semi-transparan */
    color: #fff; /* Warna teks */
    padding: 10px;
    text-align: center;
    opacity: 0; /* Awalnya tidak terlihat */
    transition: opacity 0.3s ease; /* Efek transisi saat hover */
}

.image-frame:hover .image-text-container {
    opacity: 1; /* Teks muncul saat hover */
}

.image-title {
    margin: 0;
    font-size: 16px; /* Ukuran font untuk judul */
}

.image-subtitle {
    margin: 0;
    font-size: 12px; /* Ukuran font untuk subjudul */
}


  .text-center {
    text-align: center;
  }

  .btn-video {
    position: relative;
    display: inline-block;
  }

  .image-text {
    position: absolute;
    bottom: -20px; /* Atur posisi teks di bawah gambar */
    left: 50%;
    transform: translateX(-50%);
    text-align: center;
    width: 100%; /* Agar teks berada di tengah */
    color: #000; /* Ubah warna teks sesuai kebutuhan */
    font-size: 14px; /* Atur ukuran font sesuai kebutuhan */
  }
</style>