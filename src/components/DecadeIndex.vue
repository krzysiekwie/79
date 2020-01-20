<template>
  <div>
    <div class="font-serif text-left leading-normal pt-16 pb-2 px-4">

        <p class="text-xl font-extrabold md:text-2xl -mb-6">krz<transition name="slide-fade"><span v-if="showName">ysztof </span></transition>wierz</span><transition name="slide-fade"><span v-if="showName">bicki</span></transition><span @click="showName = !showName" class="text-gray-500 hover:text-gray-600 text-5xl -ml-4">'79</span></p>

        <!-- <transition name="slide-fade">
        <p v-if="showName" class="text-xl font-extrabold md:text-2xl -mb-6">krzwierz<span @click="showName = !showName" class="text-gray-500 hover:text-gray-600 text-5xl -ml-4">'79</span></p>
        <p v-else class="text-xl font-extrabold md:text-2xl -mb-6">krzysztof wierzbicki<span @click="showName = !showName" class="text-gray-500 hover:text-gray-600 text-5xl -ml-4">'79</span></p>
        </transition> -->

        <p class="text-xl text-gray-800 font-thin mb-6 md:text-2xl pl-8 pt-4 leading-snug">professional translator/linguist & enthusiast programmer<br>
        been messing around with computers since the '80s:<br>
        <span class="font-semibold">from</span> ZX Spectrum+ and hex-editing savegames in the '90s,<br>
        <span class="font-semibold">through</span> Linux networking and web development when it was all about HTML, JS, CSS and PHP in the '00s,<br>
        <span class="font-semibold">to</span> Python for NLP, and Vue.js or React for web in the '10s.</p>

    </div>

    <div class="bg-2020s container flex items-center justify-center h-screen80 mx-auto">
        <blockquote class="bg-gray-800 opacity-75 rounded-lg mx-4 p-4 text-center md:p-8">
          <p class="font-serif font-bold italic text-3xl text-white">
            It's time for something new.
          </p>
        </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-6 px-4">
        <p class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-2 leading-snug">
        2020-2011 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
      </p>
      <div class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3" v-for="(webProject, index) in WebProjects" v-bind:key="index" v-if="webProject.yearMade > 2010 && webProject.yearMade <= 2020">
       <ProjectCard :webProject="webProject"/>
      </div>
  </div>

      <div class="bg-2010s container flex items-center justify-center h-screen mx-auto">
        <blockquote class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8">
          <p class="font-bold italic text-3xl">
            Making websites for fun and English language learners.
          </p>
        </blockquote>
      </div>

      <div class="font-serif text-left leading-normal py-6 px-4">
          <p class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-2 leading-snug">
          2010-2001 Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
        </p>
        <div class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3" v-for="(webProject, index) in WebProjects" v-bind:key="index" v-if="webProject.yearMade > 2000 && webProject.yearMade <= 2010">
         <ProjectCard :webProject="webProject"/>
        </div>
    </div>

    <div class="bg-2000s container flex items-center justify-center h-screen mx-auto">
        <blockquote class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8">
          <p class="font-bold italic text-3xl">
            Building a multi-apartment LAN and running a Linux server
          </p>
        </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-2 px-4">
        <p class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
        </p>
        <div class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3" v-for="(webProject, index) in WebProjects" v-bind:key="index" v-if="webProject.yearMade > 1990 && webProject.yearMade <= 2000">
         <ProjectCard :webProject="webProject"/>
       </div>
    </div>

    <div class="bg-1990s container flex items-center justify-center h-screen mx-auto">
        <blockquote class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8">
          <p class="font-bold italic text-3xl">
            Hacking savegames and MS Office.
          </p>
        </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-2 px-4">
        <p class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
        </p>
        <div class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3" v-for="(webProject, index) in WebProjects" v-bind:key="index" v-if="webProject.yearMade > 1980 && webProject.yearMade <= 1990">
         <ProjectCard :webProject="webProject"/>
       </div>
    </div>

    <div class="bg-1980s container flex items-center justify-center h-screen mx-auto">
        <blockquote class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8">
          <p class="font-bold italic text-3xl">
            Rewinding tapes at a loaned ZX Spectrum+
          </p>
        </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-2 px-4">
        <p class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dolor aperiam optio delectus cum adipisci, laudantium dolore, deserunt culpa magnam ea, consequuntur aspernatur saepe rem accusamus ullam qui voluptatum dolorem est.
        </p>
    </div>

  </div>
</template>

<script>
import ProjectCard from './ProjectCard'
export default {
  name: 'DecadeIndex',
  components: {
    ProjectCard
  },
  data() {
    return {
    showName: false,
    show: true,

    WebProjects: [
        {
          name: 'bhp-siedlce.com',
          yearMade: 2015,
          topic: 'company splashpage',
          imageUrl: '/projects/bhp-siedlce.png',
          imageAlt: 'BHP Siedlce',
        },
        {
          name: 'bhp-siedlce.com',
          yearMade: 2016,
          topic: 'company splashpage',
          imageUrl: '/projects/bhp-siedlce.png',
          imageAlt: 'BHP Siedlce',
        },
        {
          name: 'bhp-siedlce.com',
          yearMade: 2019,
          topic: 'company splashpage',
          imageUrl: '/projects/bhp-siedlce.png',
          imageAlt: 'BHP Siedlce',
        },
        {
          name: 'englisht.eu',
          yearMade: 2010,
          topic: 'company wordpress',
          imageUrl: '/projects/englisht.png',
          imageAlt: 'englisht.eu',
        },
        {
          name: 'englisht.eu',
          yearMade: 2009,
          topic: 'company wordpress',
          imageUrl: '/projects/englisht.png',
          imageAlt: 'englisht.eu',
        },
        {
          name: 'englisht.eu',
          yearMade: 2002,
          topic: 'company wordpress',
          imageUrl: '/projects/englisht.png',
          imageAlt: 'englisht.eu',
        },
        {
          name: 'webarchive.com',
          yearMade: 1995,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
        {
          name: 'webarchive.com',
          yearMade: 1998,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
        {
          name: 'webarchive.com',
          yearMade: 1991,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
        {
          name: 'webarchive.com',
          yearMade: 1993,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
        {
          name: 'webarchive.com',
          yearMade: 1990,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
        {
          name: 'webarchive.com',
          yearMade: 1989,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
        {
          name: 'webarchive.com',
          yearMade: 1981,
          topic: 'hobby html',
          imageUrl: '/projects/onet-republika.png',
          imageAlt: 'webarchive.com',
        },
      ]
  }}
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.slide-fade-enter-active {
  transition: all .8s cubic-bezier(1.0, 0.5, 0.8, 1.0);
}
.slide-fade-leave-active {
  transition: all .8s ease;
}
.slide-fade-enter, .slide-fade-leave-to
/* .slide-fade-leave-active below version 2.1.8 */ {
  /* transform: translateY(-20px); */
  opacity: 0;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
