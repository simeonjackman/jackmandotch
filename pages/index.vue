<template>
  <div>
    <div class="">
      <div class="fixed m-auto w-full h-screen flex justify-center items-center">
        <h1 class="title text-center text-gray-800">
          jackman[dot]ch
        </h1>
      </div>
      <button class="absolute text-3xl bottom-0 ml-auto mr-auto left-0 right-0 text-center outline-none" @click="scrollToElement">
        Contact me
      </button>
    </div>

    <div class="h-screen w-full bg-gray-100" />
    <div class="h-screen w-full bg-gray-200" />
    <div class="h-screen w-full bg-gray-300" />
    <div class="h-screen w-full bg-gray-400" />
    <div class="h-screen w-full bg-gray-500" />
    <div class="h-screen w-full bg-gray-600" />
    <div class="h-screen w-full bg-gray-700" />
    <div class="h-screen w-full bg-gray-800 bottom flex justify-center items-center z-10" >
      <a class="absolute text-gray-100 text-5xl outline-none" href="mailto:simeon@jackman.ch">Email</a>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    scrollToElement () {
      const el = this.$el.getElementsByClassName('bottom')[0]
      if (el) {
        el.scrollIntoView({ behavior: 'smooth' })
      } else {
        console.log('no el')
      }
    }
  }
}

</script>

<style>

.title {
  font-family:
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  letter-spacing: 1px;
}

/* width */
::-webkit-scrollbar {
  width: 5px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: #888;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555;
}
</style>
