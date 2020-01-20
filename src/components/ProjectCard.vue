<template>
 <div class="flex items-center rounded-lg bg-white shadow-lg overflow-hidden">
    <!-- <div class="relative pb-2/3">
      <img class="absolute h-full w-full object-cover" :src="webProject.imageUrl" :alt="webProject.imageAlt">
    </div> -->
    <img class="h-48 w-48 flex-shrink-0" :src="webProject.imageUrl" :alt="webProject.imageAlt">
    <div class="px-6 py-4">
      <h3 class="text-lg font-semibold text-gray-800">{{ webProject.name }}</h3>
      <p class="text-gray-600">made in: {{ webProject.yearMade }}</p>
      <div class="mt-4">
        <a href="#" class="text-indigo-500 hover:text-indigo-400 font-semibold text-sm">{{ webProject.topic }}</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['webProject'],
}
</script>
