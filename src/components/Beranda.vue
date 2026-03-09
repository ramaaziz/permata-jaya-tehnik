<template>
  <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8 justify-center">
    <v-app-bar theme="light">
      <v-app-bar-nav-icon>
        <v-img
          class="shadow-xl"
          contain
          src="@/assets/logo-pjt.png"
          width="32"
          @click="scrollToBottom"
        ></v-img>
      </v-app-bar-nav-icon>
      <v-app-bar-title
        class="mr-2 font-mono font-bold ml-2 text-lg shadow-2xl cursor-pointer"
        @click="scrollToBottom"
      >
        Permata Jaya Tehnik
      </v-app-bar-title>
    </v-app-bar>
    <v-main>
      <div class="mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <v-card
          class="mt-16 d-flex align-center max-w-full mx-auto shadow-2xl"
          image="@/assets/Grid2.png"
          rounded="3xl"
          :height="$vuetify.display.mdAndUp ? 450 : 150"
        >
          >
          <v-row
            align="center"
            class="ma-0 fill-height"
          >
            <v-col
              class="px-4 py-10 pl-md-10 pt-md-40"
              cols="12"
              md="6"
            >
              <div class="text-black hidden md:block">
                <h2
                  class="text-xl font-mono font-black mb-4 tracking-tight md:block sm:block"
                >
                  PT PERMATA JAYA TEHNIK
                </h2>

                <p
                  class="text-sm text-md-md italic font-mono font-medium leading-relaxed hidden-sm-and-down"
                >
                  Menghubungkan Energi, Membangun Negeri.<br />
                  Kami adalah mitra terpercaya dalam bidang<br />
                  Jasa Konstruksi dan Perdagangan Umum,<br />
                  spesialis dalam pembangunan Tower SUTET dan Jasa<br />
                  Penarikan Kabel Konduktor PLN.
                </p>
              </div>
            </v-col>
          </v-row>
        </v-card>

        <div class="mb-8 mt-8 text-center w-full">
          <h1 class="text-2xl font-heading font-bold">Visi</h1>
          <div class="font-bold text-lg -mb-1">
            PT PERMATA JAYA TEHNIK menjadi mitra kerja terpercaya
          </div>
          <h1 class="mt-8 text-2xl font-heading font-bold">Misi</h1>
          <div class="font-bold text-lg -mb-1">
            Menempatkan kepuasan mitra sebagai komitmen utama
          </div>
          <div class="font-bold text-lg mb-20">
            Memberikan kenyamanan terhadap pelanggan dengan memberikan qualitas
            terbaik
          </div>
        </div>
        <v-row class="text-left">
          <v-col
            class="text-left ml-4 mb-6"
            cols="12"
          >
            <h2 class="text-h4 font-weight-black uppercase tracking-widest">
              Sertifikasi &
              <span class="text-red-darken-1">Standar Kualitas</span>
            </h2>
            <v-divider
              class="mt-2"
              color="info"
              thickness="4"
              width="310"
            ></v-divider>
          </v-col>
        </v-row>

        <v-row
          class="m-4"
          justify="center"
        >
          <v-col
            cols="12"
            md="4"
          >
            <v-card
              border
              class="pa-6 text-center fill-height"
              flat
              height="250"
              hover
              rounded="xl"
              @click="dialog1 = true"
            >
              <v-avatar
                class="mb-4 mt-2"
                color="blue-darken-4"
                size="80"
              >
                <v-icon
                  color="white"
                  size="40"
                  >mdi-certificate
                </v-icon>
              </v-avatar>
              <v-card-title class="text-h5 font-weight-bold justify-center">
                ISO 9001:2015
              </v-card-title>
              <v-card-subtitle class="mt-2 text-wrap">
                Sistem Manajemen Mutu
              </v-card-subtitle>
              <v-card-text class="text-body-2 ml-2 mr-2 mb-2">
                Standar internasional untuk memastikan layanan konstruksi kami
                memenuhi kebutuhan klien melalui sistem manajemen kualitas yang
                efektif.
              </v-card-text>
            </v-card>
          </v-col>

          <v-col
            cols="12"
            md="4"
          >
            <v-card
              border
              class="pa-6 text-center fill-height"
              flat
              height="250"
              hover
              rounded="xl"
              @click="dialog2 = true"
            >
              <v-avatar
                class="mb-4 mt-2"
                color="green-darken-3"
                size="80"
              >
                <v-icon
                  color="white"
                  size="40"
                >
                  mdi-leaf
                </v-icon>
              </v-avatar>
              <v-card-title class="text-h5 font-weight-bold justify-center">
                ISO 14001:2015
              </v-card-title>
              <v-card-subtitle class="mt-2 text-wrap">
                Sistem Manajemen Lingkungan
              </v-card-subtitle>
              <v-card-text class="text-body-2 ml-2 mr-2 mb-2">
                Komitmen kami dalam mengelola tanggung jawab lingkungan selama
                proses pembangunan infrastruktur kelistrikan dan SUTET.
              </v-card-text>
            </v-card>
          </v-col>

          <v-col
            cols="12"
            md="4"
          >
            <v-card
              border
              class="pa-6 text-center fill-height"
              flat
              height="250"
              hover
              rounded="xl"
              @click="dialog3 = true"
            >
              <v-avatar
                class="mb-4 mt-2"
                color="orange-darken-3"
                size="80"
              >
                <v-icon
                  color="white"
                  size="40"
                >
                  mdi-hard-hat
                </v-icon>
              </v-avatar>
              <v-card-title class="text-h5 font-weight-bold justify-center">
                ISO 45001:2018
              </v-card-title>
              <v-card-subtitle class="mt-2 text-wrap">
                Manajemen Kesehatan & Keselamatan Kerja
              </v-card-subtitle>
              <v-card-text class="text-body-2 ml-2 mr-2 mb-2">
                Prioritas utama kami adalah keselamatan tenaga ahli lapangan
                dalam setiap proyek penarikan kabel konduktor dan pembangunan
                tower.
              </v-card-text>
            </v-card>
          </v-col>
          <v-dialog
            v-model="dialog1"
            :width="$vuetify.display.mdAndUp ? 600 : 300"
          >
            <v-card
              flat
              :width="$vuetify.display.mdAndUp ? 600 : 300"
            >
              <v-img
                aspect-ratio="16/9"
                cover
                src="@/assets/ISO9001.png"
                @click="dialog1 = false"
              ></v-img>
            </v-card>
          </v-dialog>
          <v-dialog
            v-model="dialog2"
            :width="$vuetify.display.mdAndUp ? 600 : 300"
          >
            <v-card
              flat
              :width="$vuetify.display.mdAndUp ? 600 : 300"
            >
              <v-img
                aspect-ratio="16/9"
                cover
                src="@/assets/ISO14001.png"
                @click="dialog2 = false"
              ></v-img>
            </v-card>
          </v-dialog>
          <v-dialog
            v-model="dialog3"
            :width="$vuetify.display.mdAndUp ? 600 : 300"
          >
            <v-card
              flat
              :width="$vuetify.display.mdAndUp ? 600 : 300"
            >
              <v-img
                aspect-ratio="16/9"
                cover
                src="@/assets/ISO45001.png"
                @click="dialog3 = false"
              ></v-img>
            </v-card>
          </v-dialog>
        </v-row>

        <v-row class="text-left">
          <v-col
            class="text-left ml-4 mb-6 mt-12"
            cols="12"
          >
            <h2 class="text-h4 font-weight-black uppercase tracking-widest">
              Project Experience & Milestones
            </h2>
            <v-divider
              class="mt-2"
              color="info"
              thickness="4"
              width="310"
            >
            </v-divider>
          </v-col>
        </v-row>

        <v-row class="text-left mx-4 mb-6 mt-4">
          <v-carousel
            aspect-ratio="16/9"
            class="rounded-xl mx-auto"
            cycle
            :height="$vuetify.display.mdAndUp ? 750 : 250"
            progress="primary"
            show-arrows="hover"
            width="fit-content"
          >
            <v-carousel-item
              contain
              src="@/assets/project1.jpeg"
            ></v-carousel-item>

            <v-carousel-item
              contain
              src="@/assets/project2.jpeg"
            ></v-carousel-item>

            <v-carousel-item
              contain
              src="@/assets/project3.jpeg"
            ></v-carousel-item>

            <v-carousel-item
              cover
              src="@/assets/project4.jpeg"
            >
            </v-carousel-item>

            <v-carousel-item
              class="object-cover"
              src="@/assets/project5.jpeg"
            >
            </v-carousel-item>

            <v-carousel-item
              contain
              src="@/assets/project6.jpeg"
            >
            </v-carousel-item>

            <v-carousel-item
              contain
              src="@/assets/project7.jpeg"
            >
            </v-carousel-item>

            <v-carousel-item
              contain
              src="@/assets/project8.jpeg"
            >
            </v-carousel-item>

            <v-carousel-item
              contain
              src="@/assets/project9.jpeg"
            >
            </v-carousel-item>
          </v-carousel>
        </v-row>

        <v-row class="text-left">
          <v-col
            class="text-left ml-4 mb-6 mt-12"
            cols="12"
          >
            <h2 class="text-h4 font-weight-black uppercase tracking-widest">
              Our Team & Expertise
            </h2>
            <v-divider
              class="mt-2"
              color="info"
              thickness="4"
              width="310"
            >
            </v-divider>
          </v-col>
        </v-row>

        <v-row
          align="center"
          justify="center"
        >
          <v-col cols="4">
            <v-carousel
              class="rounded-xl mx-auto"
              cycle
              :height="$vuetify.display.mdAndUp ? 650 : 250"
              hide-delimiters
              progress="primary"
              show-arrows="hover"
              width="fit-content"
            >
              <v-carousel-item
                contain
                src="@/assets/team2.jpg"
              ></v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team1.jpg"
              ></v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team3.jpg"
              ></v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team4.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team5.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team6.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team7.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team8.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team9.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team10.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team11.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team12.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team13.jpg"
              ></v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team14.jpg"
              ></v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team15.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team16.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team17.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team18.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team19.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team20.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team21.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team22.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team23.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team24.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team25.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team26.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team27.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team28.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team29.jpg"
              >
              </v-carousel-item>

              <v-carousel-item
                contain
                src="@/assets/team30.jpg"
              >
              </v-carousel-item>
            </v-carousel>
          </v-col>
        </v-row>

        <v-row class="text-left">
          <v-col
            class="text-left ml-4 mb-6 mt-12"
            cols="12"
          >
            <h2 class="text-h4 font-weight-black uppercase tracking-widest">
              Contact Information & Partnerships
            </h2>
            <v-divider
              class="mt-2"
              color="info"
              thickness="4"
              width="310"
            >
            </v-divider>
          </v-col>
        </v-row>

        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="12"
            sm="6"
            md="4"
          >
            <iframe
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d669.154127078746!2d107.66899595119986!3d-6.917652982295999!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e68e78b66eecc11%3A0x6d195f5f0829301c!2sPT%20PERMATA%20JAYA%20TEHNIK%2FDAFFA%20TOURS!5e1!3m2!1sen!2sid!4v1773024067406!5m2!1sen!2sid"
              width="100%"
              :height="$vuetify.display.mdAndUp ? 350 : 150"
              style="border: 0"
              loading="lazy"
              class="rounded-xl shadow-lg mb-6"
            ></iframe>
          </v-col>
        </v-row>
        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="12"
            sm="6"
            md="4"
          >
            <div class="text-center">
              <h2
                class="text-h6 text-md-h5 text-sm-h2 font-mono font-weight-black mb-3"
              >
                PT PERMATA JAYA TEHNIK
              </h2>

              <p
                class="text-caption text-md-body-1 italic font-mono leading-relaxed"
              >
                RUKO BUMI MAS KENCANA <br />
                JL. TERUSAN JAKARTA, RUKO PURI DAGO <br />
                KAV B NO.6 RT007 RW015 SUKAMISKIN <br />
                ARCAMANIK, KOTA BANDUNG-40291 <br />
                022 – 63196046 <br />
                <br />
                permatajayatehnik2019@gmail.com <br />
                permatajayatehnik89@gmail.com
              </p>
            </div>
          </v-col>
        </v-row>
      </div>
    </v-main>
  </div>
</template>

<script setup lang="ts">
import { ref } from "vue";
import { useGoTo } from "vuetify";

const dialog1 = ref(false);
const dialog2 = ref(false);
const dialog3 = ref(false);
const goTo = useGoTo();
const scrollToBottom = () => {
  goTo(document.body.scrollHeight, {
    duration: 500,
    easing: "easeInOutCubic",
  });
};
</script>
