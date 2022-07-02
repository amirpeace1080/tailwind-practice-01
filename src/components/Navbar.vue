<template>
  <div class="flex flex-wrap sm:flex-nowrap sm:justify-start p-4 items-center justify-between text-white bg-gray-700 w-full">
<!--    logo-->
    <a href="#" class="text-xl">LOGO</a>
<!--    hamberger menu-->
    <button @click="showlist" class="border border-gray-300 p-2 sm:hidden">
      <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
        <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16m-7 6h7" />
      </svg>
    </button>
<!--    list-->
    <ul v-show="list" class="list-none flex flex-col w-full sm:flex-row sm:w-auto gap-4 text-lg font-medium bg-gray-500 overflow-hidden">
      <li>First</li>
      <li>Second</li>
      <li>Third</li>
      <li>Fourd</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  data() {
    return{
      list: false,
    }
  },
  methods: {
    showlist() {
      this.list = ! this.list
    }
  }
}
</script>

<style scoped>

</style>