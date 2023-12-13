<script setup>

import '../src/assets/main.css'
import '../src/assets/variables.css'
import SaleBanner from '../src/components/SaleBanner.vue'
import NavBarTop from '../src/components/Navbar-Plaque.vue'
import Header from './components/Header-Block.vue'
import PartnersBlock from './components/partners-block.vue'
import VideoBlock from './components/Video-Block.vue'

import BenefitsBlock from './components/Benefits-Block.vue'
import OurCourses from './components/Our-Courses.vue'
import Testimonials from './components/Testimonials-Block.vue'
import Pricing from './components/Pricing-block.vue'

import Footer from './components/footer-block.vue'
import Faq from "./components/faq-block.vue"


</script>

<template>
  <body id="app">
    <SaleBanner></SaleBanner>
    

    <main class="mb-10">
      <NavBarTop></NavBarTop>
      <Header></Header>
      <PartnersBlock></PartnersBlock>
      <VideoBlock></VideoBlock>
      <BenefitsBlock></BenefitsBlock>
      <OurCourses></OurCourses>
      <Testimonials></Testimonials>
      <Pricing></Pricing>
      <Faq></Faq>
    </main>

    <footer class="">
      <Footer></Footer>
    </footer>
  </body>
</template>

<style></style>
