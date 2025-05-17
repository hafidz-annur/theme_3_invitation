<script setup>
const props = defineProps({ quote: Object });
</script>
<template>
  <v-container class="relative p-0">
    <div class="flex items-center justify-center bg-white/80 px-5 py-20">
      <div class="text-center" data-aos="zoom-in" data-aos-delay="500">
        <p class="text-[14px] text-gray-800">
          {{ props.quote?.islam[1].quote }}
        </p>
        <h3 class="text-xl font-bold mt-3">
          {{ props.quote?.islam[1].sumber }}
        </h3>
      </div>
    </div>
  </v-container>
</template>
