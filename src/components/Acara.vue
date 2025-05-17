<script setup>
import moment from "moment";

const props = defineProps({ data: Object });
</script>
<template>
  <v-container height="75vh" class="relative p-0 overflow-hidden">
    <img :src="props.data?.foto_opening" alt="Amantrana" class="w-full h-full object-cover" />
    <div class="absolute top-0 left-0 w-full h-full bg-black/70 py-10">
      <div class="flex justify-center items-center px-5">
        <div class="text-center w-full">
          <p class="mb-10" data-aos="zoom-in" data-aos-delay="500">
            Bergabunglah bersama Kami menyaksikan sekaligus merayakan
            terbentuknya ikatan suci ini. Kami ingin Anda menjadi bagian dari
            hari istimewa kami.
          </p>
          <v-card rounded="lg" class="mb-10" data-aos="fade-right" data-aos-delay="1000">
            <v-row class="items-center" no-gutters="">
              <v-col md="2" cols="3" class="bg-white flex justify-center text-center">
                <v-icon
                  color="primary"
                  icon="mdi-book-heart-outline"
                  class="-rotate-90 -mr-[25px]"
                ></v-icon>
                <h4 class="-rotate-90 font-bold text-nowrap -mr-[20px]">
                  Akad Nikah
                </h4>
              </v-col>
              <v-col md="10" cols="9" class="bg-primary py-3 px-5 text-start">
                <div class="flex items-center">
                  <v-icon icon="mdi-calendar-heart"></v-icon>
                  <div class="ms-3">
                    <p class="mb-0 text-xl font-bold">
                      {{ props.data?.acara?.akad_nikah?.hari }}
                    </p>
                    <p class="font-bold">
                      {{ props.data?.acara?.akad_nikah?.tanggal }}
                    </p>
                    <p>Pukul {{ props.data?.acara?.akad_nikah?.waktu }}</p>
                  </div>
                </div>
                <hr class="my-1" />
                <div class="flex items-center">
                  <v-icon icon="mdi-store-marker"></v-icon>
                  <p class="ms-3">
                    {{ props.data?.acara?.akad_nikah?.tempat }}
                  </p>
                </div>
              </v-col>
            </v-row>
          </v-card>

          <v-card rounded="lg" data-aos="fade-left" data-aos-delay="1500">
            <v-row class="items-center" no-gutters="">
              <v-col md="10" cols="9" class="bg-primary py-3 px-5 text-start">
                <div class="flex items-center justify-end">
                  <div class="me-3 text-end">
                    <p class="mb-0 text-xl font-bold">
                      {{ props.data?.acara?.akad_nikah?.hari }}
                    </p>
                    <p class="font-bold">
                      {{ props.data?.acara?.akad_nikah?.tanggal }}
                    </p>
                    <p>Pukul {{ props.data?.acara?.akad_nikah?.waktu }}</p>
                  </div>
                  <v-icon icon="mdi-calendar-heart"></v-icon>
                </div>
                <hr class="my-1" />
                <div class="flex items-center justify-end">
                  <p class="me-3 text-end">
                    {{ props.data?.acara?.akad_nikah?.tempat }}
                  </p>
                  <v-icon icon="mdi-store-marker"></v-icon>
                </div>
              </v-col>
              <v-col md="2" cols="3" class="bg-white flex justify-center text-center">
                <h4 class="rotate-90 font-bold text-nowrap -ml-[20px]">
                  Resepsi
                </h4>
                <v-icon
                  color="primary"
                  icon="mdi-email-open-heart-outline"
                  class="rotate-90 -ml-[15px]"
                ></v-icon>
              </v-col>
            </v-row>
          </v-card>
        </div>
      </div>
    </div>
  </v-container>
</template>
