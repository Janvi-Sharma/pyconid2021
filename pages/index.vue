<template>
  <div>
    <Hero />
    <div class="bg-white">
      <div class="max-w-7xl mx-auto py-16 px-4 sm:py-24 sm:px-6 lg:px-8">
        <div class="lg:flex lg:justify-between lg:gap-x-10">
          <div class="pb-3 lg:pb-0 max-w-xl">
            <img class="w-full h-auto rounded-lg" src="https://ik.imagekit.io/9rpt33mvmla/pyconid.jpg" alt="pycon id">
          </div>
          <div class="max-w-2xl">
            <h2 class="text-4xl font-extrabold text-gray-900 sm:text-5xl sm:tracking-tight lg:text-6xl lg:text-left">
              What is <span class="text-primary-500">PyCon ID</span>?
            </h2>
            <p class="mt-3 lg:mt-5 text-base text-gray-500 text-justify">
              Python is everywhere. It's in your favorite apps, it's used in companies worldwide, it even runs governments. Python has massive impact, not only in computing world, but the entire world. PyCon ID returns with renewed spirit to promote Python Everywhere, this is our theme for PyCon ID in 2021. We invite everyone from all walks of life to share their experience with Python. Join us to promote Python Everywhere.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="bg-white overflow-hidden">
      <div class="relative max-w-7xl mx-auto py-16 px-4 sm:px-6 lq:px-8">
        <div class="hidden lg:block bg-gray-50 absolute top-0 bottom-0 left-3/4 w-screen" />
        <div class="mx-auto text-base max-w-prose lg:grid lg:grid-cols-2 lg:gap-8 lg:max-w-none">
          <div>
            <h3 class="mt-2 mb-4 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
              Keynote Speaker
            </h3>
          </div>
        </div>
        <KeynoteSpeaker shadow="sm" />
      </div>
    </div>
    <SNS />
    <div>
      <YoutubePlaylist />
    </div>
  </div>
</template>

<script>
import Hero from '@/components/homepage/Hero.vue'
import SNS from '@/components/global/SNS.vue'
import YoutubePlaylist from '@/components/homepage/YoutubePlaylist.vue'
import KeynoteSpeaker from '@/components/global/KeynoteSpeaker.vue'

export default {
  components: {
    Hero,
    SNS,
    YoutubePlaylist,
    KeynoteSpeaker
  },
  head () {
    return {
      script: [
        { hid: 'twitter', src: 'https://platform.twitter.com/widgets.js', defer: true },
        { hid: 'instagram', src: '//www.instagram.com/embed.js', defer: true }
      ]
    }
  }
}
</script>
