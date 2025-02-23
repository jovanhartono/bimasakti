<script setup lang="ts">
import GlobeComponent from '@/components/GlobeComponent.vue'
import { ORBIT_DIRECTION } from '@/components/orbit'
import Orbit from '@/components/orbit/OrbitComponent.vue'

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
        <div class="shrink-0 text-6xl font-medium tracking-tight">
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
        <h2 class="shrink-0 text-lg font-medium tracking-tight">ABOUT US</h2>
        <div class="col-span-2">
          <p>
            PT Bima Sakti Nawasena Sentosa adalah perusahaan General Trading yang berdedikasi untuk
            memberikan solusi inovatif dalam berbagai sektor, termasuk produk property, produk
            Investasi, dan Produk Technology.
          </p>
          <p class="mt-2">
            Perusahaan ini fokus pada pembelian, penyewaan, serta pengelolaan properti komersial dan
            industri, dengan tujuan untuk mendukung perkembangan bisnis serta meningkatkan nilai
            investasi klien. Sejak berdiri, PT Bima Sakti Nawasena Sentosa telah menjadi pemain
            utama di pasar dengan komitmen untuk terus mengembangkan diri dan memenuhi kebutuhan
            pasar yang dinamis.
          </p>
        </div>
      </div>
    </section>

    <!-- property -->
    <section class="container grid gap-4 sm:grid-cols-7">
      <div class="col-span-3">
        <h1 class="text-3xl font-medium text-balance">
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

    <section class="container flex flex-col gap-y-6">
      <div class="flex flex-col items-center">
        <h1 class="text-center text-4xl font-medium text-balance">
          <span class="font-handwriting align-middle text-6xl font-bold text-amber-900">
            Precious
          </span>
          Metals Trading
        </h1>
        <p class="mt-2 text-center text-balance">
          Menyediakan layanan pembelian, penjualan, dan investasi logam mulia seperti emas dan
          perak, yang dapat menjadi alternatif investasi jangka panjang yang aman dan menguntungkan.
          Dengan pengalaman di pasar logam mulia, PT Bimasakti Nawasena Sentosa memastikan produk
          yang dijual memiliki kualitas terbaik serta memberikan jaminan bagi para investor.
        </p>
      </div>
      <div class="relative flex h-[500px] flex-col items-center justify-center">
        <img
          loading="lazy"
          decoding="async"
          src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPczPzdrjue8RPKOD2CnAfwGUZVdkbBLaTM1SN"
          alt="gold hand"
          class="h-[200px] w-auto object-contain sm:h-[250px]"
        />

        <Orbit
          path
          class="size-14 items-center justify-center border-none bg-transparent"
          :duration="40"
          :radius="150"
          :direction="ORBIT_DIRECTION.CounterClockwise"
        >
          <img
            loading="lazy"
            decoding="async"
            src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPi0bzu6sGTWmQc716zsqCXZxAo0ehNdJOrj3l"
            alt="platinum nugget"
          /> </Orbit
        ><Orbit
          path
          class="size-16 items-center justify-center border-none bg-transparent"
          :radius="190"
          :duration="20"
          :direction="ORBIT_DIRECTION.Clockwise"
        >
          <img
            loading="lazy"
            decoding="async"
            src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPKaZW5g1HBhyQbeCRGNZt0UP57daFTruIXJpD"
            alt="silver nugget"
          /> </Orbit
        ><Orbit
          path
          class="size-16 items-center justify-center border-none bg-transparent"
          :delay="60"
          :radius="250"
          :direction="ORBIT_DIRECTION.CounterClockwise"
        >
          <img
            loading="lazy"
            decoding="async"
            src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPkDg5XQMfg4KV6QXDxA8ebpvOj9J23HTZMYhL"
            alt="gold nugget"
          />
        </Orbit>
      </div>
    </section>

    <section class="container flex flex-col items-center rounded-sm p-6">
      <dl class="text-center">
        <dt class="text-4xl font-medium">Software Powerhouse</dt>
        <dd class="mt-2 text-balance opacity-70">
          Menyediakan penjualan dan penyewaan perangkat lunak serta perangkat keras industri,
          termasuk AI, untuk mendukung operasional bisnis, manufaktur, distribusi, dan logistik
          dengan teknologi efisien dan terjangkau.
        </dd>
      </dl>

      <video
        autoplay
        muted
        loop
        loading="lazy"
        decoding="async"
        src="https://xnxk060v5p.ufs.sh/f/D0ooyPBt8scPxARYj1utnmtRG1PuprOAyJDeMHlg3s9k4Wc5"
        class="mt-6 w-[350px] object-contain object-center"
        preload="none"
        playsinline
        draggable="false"
        disablePictureInPicture
        disableRemotePlayback
      />
    </section>

    <!-- company vision -->
    <section class="container flex flex-col">
      <h1 class="text-center text-4xl leading-normal font-medium">
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
          <div class="flex flex-col gap-4">
            <a class="flex flex-col gap-y-2 text-left" href="tel:+6281234567890">
              <span class="font-medium hover:underline">+62 812-3456-7890</span>
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
