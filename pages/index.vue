<template>
  <div>
    <div class="m-auto w-full h-screen flex flex-col justify-center items-center">
      <h1 class="title text-center text-gray-800 text-3xl md:text-6xl">
          jackman[dot]ch
      </h1>
      <button class="cursor-pointer text-centertext-gray-800  outline-none text-l md:text-xl" @click="scrollToElement">
        More info
      </button>
    </div>

    <div class="h-screen w-full bg-gray-100 relative" />
    <div class="h-screen w-full bg-gray-200 relative" />
    <div class="h-screen w-full bg-gray-300 relative" />
    <div class="h-screen w-full bg-gray-400 relative" />
    <div class="h-screen w-full bg-gray-500 relative" />
    <div class="h-screen w-full bg-gray-600 relative" />
    <div class="h-screen w-full bg-gray-700 relative" />
    <div class="h-screen w-full bg-gray-800 bottom flex justify-center items-center" >
      <div class="m-auto">
        <div class="flex items-center py-2">
          <svg viewBox="0 0 20 20" class="text-gray-100 fill-current h-8 w-8">
            <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z" />
            <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z" />
          </svg>
          <a class="px-2 text-gray-100 outline-none text-xl md:text-3xl" href="mailto:simeon@jackman.ch">[Send] me an email</a>
        </div>
        <div class="flex items-center py-2">
          <svg viewBox="0 0 24 24" class="text-gray-100 fill-current h-8 w-8">
            <path fill-rule="evenodd" clip-rule="evenodd" d="M12 2C6.477 2 2 6.463 2 11.97c0 4.404 2.865 8.14 6.839 9.458.5.092.682-.216.682-.48 0-.236-.008-.864-.013-1.695-2.782.602-3.369-1.337-3.369-1.337-.454-1.151-1.11-1.458-1.11-1.458-.908-.618.069-.606.069-.606 1.003.07 1.531 1.027 1.531 1.027.892 1.524 2.341 1.084 2.91.828.092-.643.35-1.083.636-1.332-2.22-.251-4.555-1.107-4.555-4.927 0-1.088.39-1.979 1.029-2.675-.103-.252-.446-1.266.098-2.638 0 0 .84-.268 2.75 1.022A9.606 9.606 0 0112 6.82c.85.004 1.705.114 2.504.336 1.909-1.29 2.747-1.022 2.747-1.022.546 1.372.202 2.386.1 2.638.64.696 1.028 1.587 1.028 2.675 0 3.83-2.339 4.673-4.566 4.92.359.307.678.915.678 1.846 0 1.332-.012 2.407-.012 2.734 0 .267.18.577.688.48C19.137 20.107 22 16.373 22 11.969 22 6.463 17.522 2 12 2z"></path>
          </svg>
          <a class="px-2 text-gray-100 outline-none text-xl md:text-3xl" target="_blank" rel="noopener noreferrer" href="https://github.com/simeonjackman">[Checkout] my github</a>
        </div>
        <div class="flex items-center py-2">
          <svg viewBox="0 0 20 20" class="text-gray-100 fill-current h-8 w-8">
            <path d="M9 4.804A7.968 7.968 0 005.5 4c-1.255 0-2.443.29-3.5.804v10A7.969 7.969 0 015.5 14c1.669 0 3.218.51 4.5 1.385A7.962 7.962 0 0114.5 14c1.255 0 2.443.29 3.5.804v-10A7.968 7.968 0 0014.5 4c-1.255 0-2.443.29-3.5.804V12a1 1 0 11-2 0V4.804z" />
          </svg>
          <a class="px-2 text-gray-100 outline-none text-xl md:text-3xl" target="_blank" rel="noopener noreferrer" href="http://liu.diva-portal.org/smash/record.jsf?pid=diva2%3A1323791&dswid=9098">[Read] my masters thesis</a>
        </div>
      </div>
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
