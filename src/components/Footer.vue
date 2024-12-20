<script setup>
import { contactInfo } from "../data/items";

const currentYear = new Date().getFullYear();
const isMenuOpen = false;

const column1Heading = "Nira Digital";
const column1Text =
  "Nira Digital adalah layanan jasa digital yang menawarkan berbagai solusi untuk memenuhi kebutuhan akademik dan digital. Kami menyediakan jasa pembuatan tugas dan skripsi, serta membantu mahasiswa dalam menyelesaikan pekerjaan akademik dengan kualitas terbaik. Selain itu, kami juga menawarkan layanan top-up diamond untuk berbagai game serta penyediaan akun premium untuk berbagai platform. Tidak hanya itu, Nira Digital juga ahli dalam pembuatan dan pengembangan aplikasi, serta menyediakan layanan pembuatan undangan digital yang modern dan praktis. Kami berkomitmen untuk memberikan layanan yang efisien dan dapat diandalkan sesuai dengan kebutuhan pelanggan.";
const column4Heading = "Contact";

const connectHeading = "Connect";

const socialItems = [
  {
    link: "https://www.instagram.com/",
    icon: "icon-instagram",
  },
  {
    link: "https://www.twitter.com/",
    icon: "icon-twitter",
  },
  {
    link: "https://www.facebook.com/",
    icon: "icon-facebook",
  },
];
</script>

<template>
  <div class="site-footer">
    <div class="footer-dots"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="widget">
            <h3>{{ column1Heading }}</h3>
            <p style="text-align: justify;">{{ column1Text }}</p>
          </div>
          <div class="widget">
            <h3>{{ connectHeading }}</h3>
            <ul class="list-unstyled social">
              <li style="margin-right: 4px">
                <a :href="socialItems[0].link" target="_blank">
                  <span :class="socialItems[0].icon"></span>
                </a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[1].link" target="_blank">
                  <span :class="socialItems[1].icon"></span
                ></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[2].link" target="_blank">
                  <span :class="socialItems[2].icon"></span
                ></a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-lg-2 ml-auto">
          <div class="widget">
          </div>
        </div>
        <div class="col-lg-2">
          <div class="widget">
          </div>
        </div>
        <div class="col-lg-3">
          <div class="widget">
            <h3>{{ column4Heading }}</h3>
            <address>{{ contactInfo.address }}</address>
            <ul class="list-unstyled links mb-4">
              <li>
                <a :href="'https://wa.me/' + contactInfo.phone2 + '?text=Hallo%20*Nira%20Digital*, '" target="_blank">
                  {{ contactInfo.phone2 }}
                </a>
              </li>
              <li>
                <a :href="'mailto:' + contactInfo.email" target="_blank">
                  <span>{{ contactInfo.email }}</span></a
                >
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-12 text-center">
          <p>&copy; {{ currentYear }} <a href="https://niradigital.id" target="_blank" rel="noopener noreferrer">NiraDigital</a>. All rights reserved.</p>
        </div>
      </div>
    </div>
  </div>
</template>
