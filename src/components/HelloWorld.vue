<template>
  <v-container :fluid="true">
    <v-card>
      <v-card-title>
        鳝鱼は？
      </v-card-title>
      <v-card-text>
        刘善宇，山东枣庄人也，生性嗜好同行，世人谓之曰gay。
        <v-carousel :hide-delimitersi="true" :cycle="true" :show-arrows="false">
          <v-carousel-item v-for="(banner, i) in BannerList" :key="i" :src="'/banners/' + banner.file">
          </v-carousel-item>
        </v-carousel>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script setup>
import BannerList from "@/assets/BannerList";
</script>
