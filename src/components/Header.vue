<script setup>
import { themeColor, siteName } from "../data/items";
</script>
<template>
  <nav class="site-nav dark js-site-navbar mb-5 site-navbar-target">
    <div class="container">
      <div class="site-navigation">
        <a href="" class="logo m-0 float-left"
          >{{ siteName }}<span class="text-primary">.</span></a
        >
        <ul class="js-clone-nav d-none d-lg-inline-block site-menu float-left">
          <li class="active">
            <a href="#home-section" class="nav-link">Home</a>
          </li>
          <li><a href="#jasa-section" class="nav-link">Jasa Tugas</a></li>
          <li><a href="#topup-section" class="nav-link">TopUp Diamond & Streaming</a></li>
          <li><a href="#undangan-section" class="nav-link">Undangan Digital</a></li>
          <li><a href="#apk-section" class="nav-link">Aplikasi</a></li>
          <li><a href="#sc-section" class="nav-link">Source Code</a></li>
          <li><a href="#contact-section" class="nav-link">Contact</a></li>
        </ul>
        <a
          href="#"
          class="burger ml-auto float-right site-menu-toggle js-menu-toggle d-inline-block dark d-lg-none"
          data-toggle="collapse"
          data-target="#main-navbar"
        >
          <span></span>
        </a>
      </div>
    </div>
  </nav>
</template>
