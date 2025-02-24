<script setup lang="ts">
import GlobeComponent from '@/components/GlobeComponent.vue'
import { ORBIT_DIRECTION } from '@/components/orbit'
import Orbit from '@/components/orbit/OrbitComponent.vue'
import { PhoneIcon, MailIcon } from 'lucide-vue-next'
const propertyImages = [
  'https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPUTxm5Xq8flCdQOAPv1XWbw5rVGjp3KkJEiSD',
  'https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPl26BD39AV0pmdhg1jn8rSqJbE9CF4HiUGDXN',
  'https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPmw4CkU1ProDmsk0lfqcZuEAe93hGi1YdQWav',
]
</script>

<template>
  <main class="flex flex-col gap-y-8 sm:gap-y-12">
    <div class="container mx-auto flex items-center pt-6 sm:pt-12">
      <div class="flex gap-4 max-sm:flex-col">
        <div class="shrink-0 text-6xl font-medium tracking-tight text-blue-950">
          Connecting Markets
          <span class="block">
            <span
              class="font-handwriting bg-gradient-brand align-middle font-bold tracking-tighter sm:tracking-wide"
            >
              Empowering
            </span>
            Businesses
          </span>
        </div>
        <p class="mt-auto mb-2 text-left text-pretty sm:text-right">
          Bergerak di bidang properti, logam mulia, dan industri, dengan fokus pada pembelian,
          penyewaan, dan pengelolaan aset.
        </p>
      </div>
    </div>

    <section class="flex flex-col gap-y-4">
      <img
        loading="eager"
        src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPKMf7cOE1HBhyQbeCRGNZt0UP57daFTruIXJp"
        alt="gold background"
        decoding="async"
        fetchpriority="high"
        class="container h-[350px] object-cover sm:h-[500px]"
      />

      <!-- about us -->
      <div class="container grid justify-between gap-x-4 gap-y-1 sm:grid-cols-3" id="about">
        <h2 class="shrink-0 text-lg font-semibold tracking-tight text-blue-950">ABOUT US</h2>
        <div class="col-span-2">
          <p>
            PT Bimasakti Nawasena Sentosa adalah perusahaan General Trading yang berdedikasi untuk
            memberikan solusi inovatif dalam berbagai sektor, termasuk produk property, produk
            Investasi, dan produk <i>technology.</i>
          </p>
          <p class="mt-2">
            Perusahaan ini fokus pada pembelian, penyewaan, serta pengelolaan properti komersial dan
            industri, dengan tujuan untuk mendukung perkembangan bisnis serta meningkatkan nilai
            investasi klien. Sejak berdiri, PT Bimasakti Nawasena Sentosa telah menjadi pemain utama
            di pasar dengan komitmen untuk terus mengembangkan diri dan memenuhi kebutuhan pasar
            yang dinamis.
          </p>
        </div>
      </div>
    </section>

    <!-- property -->
    <section class="container grid gap-4 sm:grid-cols-7">
      <div class="col-span-3">
        <h1 class="text-3xl font-medium text-blue-950 sm:text-balance">
          Strategic Property Solutions for Business Growth
        </h1>
        <p class="mt-2">
          Menawarkan layanan pembelian dan penyewaan properti komersial dan industri, seperti gedung
          perkantoran, pabrik, dan gudang. Setiap properti dirancang untuk memberikan kenyamanan
          serta efisiensi operasional yang optimal.
        </p>
      </div>
      <div
        class="col-span-4 flex touch-pan-x snap-x snap-mandatory gap-x-4 overflow-x-auto *:snap-start"
      >
        <img
          v-for="image in propertyImages"
          :key="image"
          :width="400"
          :height="550"
          :src="image"
          alt="office"
          loading="lazy"
          decoding="async"
          class="h-[450px] w-[325px] shrink-0 object-cover sm:h-[550px] sm:w-[400px]"
        />
      </div>
    </section>

    <section class="relative container grid gap-4 max-sm:h-[400px] max-sm:flex-col sm:grid-cols-7">
      <div class="absolute inset-0 z-10 bg-black/50 sm:hidden"></div>

      <div class="z-20 mt-12 flex flex-col sm:col-span-3 sm:mt-0">
        <h1 class="text-4xl font-medium text-white sm:text-blue-950">Precious Metals Trading</h1>
        <p class="mt-2 text-balance max-sm:text-white max-sm:opacity-100">
          Menyediakan layanan pembelian, penjualan, dan investasi logam mulia seperti emas dan
          perak, yang dapat menjadi alternatif investasi jangka panjang yang aman dan menguntungkan.
          Dengan pengalaman di pasar logam mulia, PT Bimasakti Nawasena Sentosa memastikan produk
          yang dijual memiliki kualitas terbaik serta memberikan jaminan bagi para investor.
        </p>
      </div>
      <img
        src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPa7MR3DznJFzv6W8Th1gH7crLuOGQNyfw2Ret"
        alt="gold background"
        loading="lazy"
        decoding="async"
        class="z-0 h-full object-cover max-sm:absolute max-sm:inset-0 sm:col-span-4 sm:aspect-square"
      />
    </section>

    <section class="container flex flex-col items-center rounded-sm p-6">
      <dl class="text-center">
        <dt class="text-4xl font-medium text-blue-950">Software Powerhouse</dt>
        <dd class="mt-2 text-balance opacity-70">
          Menyediakan penjualan dan penyewaan perangkat lunak serta perangkat keras industri,
          termasuk <i>AI</i>, untuk mendukung operasional bisnis, manufaktur, distribusi, dan
          logistik dengan teknologi efisien dan terjangkau.
        </dd>
      </dl>
      <video
        autoplay
        muted
        loop
        loading="eager"
        decoding="async"
        src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPxARYj1utnmtRG1PuprOAyJDeMHlg3s9k4Wc5"
        class="mt-6 w-[350px] object-contain object-center"
        playsinline
        draggable="false"
        disablePictureInPicture
        disableRemotePlayback
      />
    </section>

    <!-- company vision -->
    <section class="container flex flex-col">
      <h1 class="text-center text-4xl leading-snug font-medium text-blue-950">
        Our Vision – A Glimpse Into the Future
      </h1>
      <p class="mt-2 text-center text-balance">
        PT Bimasakti Nawasena Sentosa bertekad menjadi pemimpin dalam perdagangan properti,
        investasi, dan teknologi. Perusahaan terus berinovasi, memperluas jaringan, dan memberikan
        layanan terbaik bagi klien. Dengan tim profesional berpengalaman, perusahaan siap menghadapi
        pasar global dan berkontribusi pada pertumbuhan ekonomi Indonesia.
      </p>
      <div class="relative h-[375px] overflow-hidden sm:h-[300px]">
        <GlobeComponent class="top-0" />
      </div>
    </section>

    <section id="contact" class="mt-6 bg-blue-950 py-6 text-white sm:py-12">
      <div class="container flex gap-4 max-sm:flex-col">
        <div class="flex flex-col gap-y-3">
          <h1 class="text-4xl font-medium">Get in Touch with Our Team</h1>
          <p class="opacity-90">
            Hubungi kami untuk mendapatkan informasi lebih lanjut tentang layanan kami dan bagaimana
            kami dapat membantu Anda mencapai tujuan bisnis Anda.
          </p>
          <div class="flex flex-col gap-2">
            <a class="flex items-center gap-x-2 text-left" href="tel:02178342780">
              <PhoneIcon class="size-4 text-white" />
              <span class="font-medium hover:underline">021-78342780</span>
            </a>
            <a
              class="flex items-center gap-x-2 text-left"
              href="mailto:bimasaktisentosa25@gmail.com"
            >
              <MailIcon class="size-4 text-white" />
              <span class="font-medium hover:underline">bimasaktisentosa25@gmail.com</span>
            </a>
          </div>
        </div>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3965.8301669419473!2d106.80962160549706!3d-6.290545955850148!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f1fa5b9f59a3%3A0x772f6f7bc1fbc6c0!2sMenara%20165!5e0!3m2!1sen!2sid!4v1740321602656!5m2!1sen!2sid"
          class="aspect-square w-full border-0"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </section>
  </main>
</template>
