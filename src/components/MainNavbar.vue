<template>
  <nav class="fixed p-2 bg-gray-100 w-screen shadow-lg z-50">
    <ul class="flex border-b">
      <li class="mr-1">
        <a
          class="
            bg-gray-100
            inline-block
            py-2
            px-4
            text-blue-500
            hover:text-blue-800
            font-semibold
          "
          href="https://krzysiekwie.github.io/"
          >krzysiekwie.github.io</a
        >
      </li>
      <li class="-mb-px mr-1">
        <router-link
          class="
            bg-gray-100
            inline-block
            border-l border-t border-r
            rounded-t
            py-2
            px-4
            text-blue-700
            font-semibold
          "
          to="/"
          >Projects</router-link
        >
      </li>
      <li class="mr-1">
        <a
          class="
            bg-gray-100
            inline-block
            py-2
            px-4
            text-blue-500
            hover:text-blue-800
            font-semibold
          "
          href="https://krzysiekwie.github.io/hugowie/"
          >Notes</a
        >
      </li>

      <!-- 
            
            <li class="mr-1">
            <a class="bg-gray-100 inline-block py-2 px-4 text-gray-400 font-semibold" href="#">Tab</a>
            </li>
        
            <li class="mr-1">
            <router-link class="bg-gray-100 inline-block py-2 px-4 text-gray-400 font-semibold" to="/about">About</router-link>
            </li> -->
    </ul>
  </nav>
</template>

<script>
export default {
  name: "MainNavbar",
  data() {
    return {};
  },
};
</script>

<style>
.navbar nav {
  padding: 0 20px;
}
</style>
