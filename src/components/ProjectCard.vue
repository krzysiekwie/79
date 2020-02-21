<template>
  <div
    v-tilt="{
      max: 10,
      speed: 200,
      perspective: 2000,
      easing: 'cubic-bezier(0.42, 0.0, 0.58, 1.0)'
      }"
    class="max-h-full mx-w-sm sm:flex items-center rounded-lg bg-white shadow-lg overflow-hidden"
  >
    <div class="sm:flex-shrink-0">
      <img
        class="mx-auto rounded-lg sm:w-48"
        :src="webProject.imageUrl"
        :alt="webProject.imageAlt"
      />
    </div>
    <div class="px-6 py-4 flex-shrink-0 text-center sm:text-left">
      <h3 class="text-4xl sm:truncate sm:text-lg font-semibold text-gray-800">
        {{ webProject.name }}
      </h3>
      <p class="text-4xl sm:truncate sm:text-lg text-gray-600">
        from: {{ webProject.yearMade }}
      </p>
      <p class="text-4xl sm:truncate sm:text-sm text-gray-700">{{ webProject.topic }}</p>
      <div class="mt-4">
        <a
          :href="webProject.projectUrl"
          class="text-4xl sm:text-lg text-md text-indigo-500 hover:text-indigo-300 font-semibold "
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
