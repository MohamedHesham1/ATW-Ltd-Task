<template>
  <div>
    <NavbarComponent />

    <HeroSection />

    <DisplaySection
      title="KattyEfa NFT"
      text="The image is a high-quality digital painting with a resolution of 5000x1250 pixels."
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
    <FooterComponent />
  </div>
</template>

<script setup>
import HeroSection from './HeroSection.vue'
import DisplaySection from './DisplaySection.vue'
import CollectionSection from './CollectionsSection.vue'
import TrendingSection from './TrendingSection.vue'
import NavbarComponent from './NavbarComponent.vue'
import FooterComponent from './FooterComponent.vue'
</script>

<style scoped></style>
