<template>
  <div
    class=" mx-w-sm md:flex items-center rounded-lg bg-white shadow-lg overflow-hidden"
  >
    <!-- working: <div class="flex items-center rounded-lg bg-white shadow-lg overflow-hidden"> -->
    <!-- <div class="relative pb-2/3">
      <img
        class="absolute h-full w-full object-cover"
        :src="webProject.imageUrl"
        :alt="webProject.imageAlt"
      />
    </div> -->
    <div class="md:flex-shrink-0">
      <img
        class="rounded-lg md:w-48"
        :src="webProject.imageUrl"
        :alt="webProject.imageAlt"
      />
    </div>
    <div class="px-6 py-4 text-center md:text-left">
      <h3 class="text-4xl md:text-lg font-semibold text-gray-800">
        {{ webProject.name }}
      </h3>
      <p class="text-4xl md:text-lg text-gray-600">
        from: {{ webProject.yearMade }}
      </p>
      <p class="text-4xl md:text-lg text-gray-500">{{ webProject.topic }}</p>
      <div class="mt-4">
        <a
          :href="webProject.projectUrl"
          class="text-4xl md:text-lg text-md text-indigo-500 hover:text-indigo-400 font-semibold "
          >Open</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["webProject"]
};
</script>
