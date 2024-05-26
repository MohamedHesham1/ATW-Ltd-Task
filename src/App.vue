<template>
  <header>
    <NavbarComponent />
  </header>

  <main>
    <HeroSection />

    <DisplaySection
      title="KattyEfa NFT"
      text="The image is a high-quality digital painting with a resolution of 5000x1250 pixels ."
      price="$1.5 million"
      imagePath="/Moddy Character NFT.png"
      height="h-[562px]"
    />

    <DisplaySection
      title="Moddy Character NFT"
      text="The image is a high-quality digital painting with a resolution of 3000x2000 pixels and is optimized for the web."
      price="$101,593"
      imagePath="/KattyEfa NFT.png"
      height="h-[539px]"
    />

    <CollectionSection />

    <TrendingSection />
  </main>

  <FooterComponent />
</template>

<script setup>
import DisplaySection from './components/DisplaySection.vue'
import HeroSection from './components/HeroSection.vue'
import NavbarComponent from './components/NavbarComponent.vue'
import CollectionSection from './components/CollectionsSection.vue'
import TrendingSection from './components/TrendingSection.vue'
import FooterComponent from './components/FooterComponent.vue'
</script>

<style scoped></style>
