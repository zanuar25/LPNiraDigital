<script setup>
import { themeColor } from "../data/items";
import mainPhoto from "../assets/images/service1.png";

const buttonWeb = "Website";
const buttonHub = "Hubungi Kami Sekarang"

const service1Heading = "Layanan Nira Digital";
const service1SubHeading = "Jasa Tugas dan Skripsi";
</script>
<template>
  <div class="untree_co-section" id="jasa-section">
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-lg-4">
          <span
            class="caption"
            data-aos="fade-up"
            data-aos-delay="0"
            :style="[{ color: themeColor }]"
            >{{ service1Heading }}</span
          >
          <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
            {{ service1SubHeading }}
          </h3>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="200">
            <p>
              Jasa Tugas dan Skripsi, solusi praktis untuk menyelesaikan tugas akademik 
              dan pekerjaan kreatif Anda! Kami adalah tim profesional yang siap membantu 
              Anda dalam mengerjakan berbagai jenis tugas, mulai dari Pengerjaan PPT & 
              Presentasi, Desain Grafis, Video Editing, Pemrograman & Pengembangan Aplikasi, 
              Penulisan Proposal, Penulisan Jurnal & Artikel, dan Bimbingan & Penulisan Skripsi. 
              Layanan kami mencakup berbagai jurusan dan topik, sehingga Anda bisa merasa tenang 
              karena pekerjaan Anda akan ditangani oleh ahli di bidangnya.
            </p>
            <p>
              <b>Kenapa Memilih Kami?</b>
            </p>
            <ul class="list-unstyled ul-check primary">
              <li>Profesinal</li>
              <li>Kualitas Terjamin</li>
              <li>Terpercaya</li>
              <li>Penyelesaian Tepat Waktu</li>
            </ul>
          </div>
        </div>
        <div class="col-lg-7" data-aos="fade-up" data-aos-delay="400">
            <img :src="mainPhoto" alt="Image" class="img-fluid img-shadow" />
        </div>
        <div style="display: flex; gap: 10px;">
          <a
            href="https://jasa.niradigital.my.id/"
            class="btn btn-primary smoothscroll"
            v-bind:style="{ background: themeColor, borderColor: themeColor }"
            target="_blank"
          >
            {{ buttonWeb }}
          </a>
          <a
              href="https://wa.me/6282213171707?text=Halo%2C%20Saya%20mau%20jasa%20rugas" 
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
