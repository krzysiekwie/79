<template>
  <div>
    <div class="font-serif text-left leading-normal pt-16 pb-2 px-4">
      <p class="text-xl font-extrabold md:text-2xl -mb-6">
        <span>krz</span
        ><transition name="slide-fade"
          ><span v-if="showName">ysztof&nbsp;</span></transition
        >
        <span>wierz</span
        ><transition name="slide-fade"
          ><span v-if="showName">bicki</span></transition
        >
        <span
          @click="showName = !showName"
          class="text-gray-500 hover:text-gray-600 text-5xl -ml-4"
          >'79</span
        >
      </p>

      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl pl-8 pt-4 leading-snug"
      >
        professional translator/linguist & enthusiast programmer
        <br />been messing around with computers since the '80s:
        <br />
        <span class="font-semibold">from</span> ZX Spectrum+ and hex-editing
        savegames in the '90s,
        <br />
        <span class="font-semibold">through</span> Linux networking and web
        development when it was all about HTML, JS, CSS and PHP in the '00s,
        <br />
        <span class="font-semibold">to</span> Python for NLP, and Vue.js or
        React for web in the '10s.
      </p>
    </div>

    <div
      class="bg-2020s container flex items-center justify-center h-screen80 mx-auto"
    >
      <blockquote
        class="bg-gray-800 opacity-75 rounded-lg mx-4 p-4 text-center md:p-8"
      >
        <p class="font-serif font-bold italic text-3xl text-white">
          It's time for something new.
        </p>
      </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-6 px-4">
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-2 leading-snug"
      >
        When I first moved my nibylog website to Wordpress I decided making
        websites is so simple now, nobody needs any help. Indeed writing in
        English for SEO seemed much better business option. Every now and then,
        I would change some old PHP at a company I worked for or .zip()
        something in Python to make a quick translation memory or terminology
        reference.
      </p>
      <div
        class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3"
        v-for="(webProject, index) in WebProjects20s"
        v-bind:key="index"
      >
        <ProjectCard :webProject="webProject" />
      </div>
    </div>

    <div
      class="bg-2010s container flex items-center justify-center h-screen mx-auto"
    >
      <blockquote
        class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8"
      >
        <p class="font-bold italic text-3xl">
          Making websites for fun and English language learners.
        </p>
      </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-6 px-4">
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-2 leading-snug"
      >
        This is when I earned my first money as a webdesigner. I've been putting
        together websites for fun, from role-playing games, through
        play-by-email, to fansites, when a local computer store decided they
        needed to upgrade their static HTML with some JS. In these pre jQuery
        days I remember my design looked pretty awesome to me, and useful enough
        to the client to pay for it. I just hoped he would not discover this new
        technology everyone was excited about, called Flash! <br />Because that
        one, I did not like...
      </p>
      <div
        class="inline-block mt-6 w-full px-4 md:w-1/2 lg:w-1/3"
        v-for="(webProject, index) in WebProjects10s"
        v-bind:key="index"
      >
        <ProjectCard :webProject="webProject" />
      </div>
    </div>

    <div
      class="bg-2000s container flex items-center justify-center h-screen mx-auto"
    >
      <blockquote
        class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8"
      >
        <p class="font-bold italic text-3xl">
          Building a multi-apartment LAN and running a Linux server
        </p>
      </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-2 px-4">
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug"
      >
        Listening to the beeps of the modem was expensive, and getting a
        dedicated broad-band connection even more so. Luckily I lived in a block
        of flats where most people felt the same. Even more lucky, my parents'
        kitchen had an empty cupboard which could be adapted to house a rack
        with FreeSCO server. Several Linux books later I was in over my head
        building and later administering a building-wide LAN sharing an SDI (S
        originally meaning Speed, later changed to Stable) connection at 115,2
        kb/s.
      </p>
      <div
        class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3"
        v-for="(webProject, index) in WebProjects00s"
        v-bind:key="index"
      >
        <ProjectCard :webProject="webProject" />
      </div>
    </div>

    <div
      class="bg-1990s container flex items-center justify-center h-screen mx-auto"
    >
      <blockquote
        class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8"
      >
        <p class="font-bold italic text-3xl">
          Hacking savegames
        </p>
      </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-2 px-4">
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug"
      >
        The 90s was a time when I graduated from a loaned Spectrum and Amiga to
        my own pen-and-paper turtle cut-out from a book on Logo programming
        language followed by Commodore 64 but it wasn't until I got my hands on
        a PC when games got boring in one afternoon when I discovered the
        wonderful world of hex-editing my savegames.
      </p>
      <div
        class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3"
        v-for="(webProject, index) in WebProjects90s"
        v-bind:key="index"
      >
        <ProjectCard :webProject="webProject" />
      </div>
    </div>

    <div
      class="bg-1980s container flex items-center justify-center h-screen mx-auto"
    >
      <blockquote
        class="bg-black opacity-50 rounded-lg font-serif mx-4 p-4 text-center text-white md:p-8"
      >
        <p class="font-bold italic text-3xl">
          Rewinding tapes at a loaned ZX Spectrum+
        </p>
      </blockquote>
    </div>

    <div class="font-serif text-left leading-normal py-2 px-4">
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug"
      >
        I only vaguely remember the quest of going to a local computer club,
        where a bespectaled, sweater-clad wizzard gave me the secret spell of
        LOAD "" that made the rolling tape do magic with the black box of
        Sinclair ZX Spectrum we had on loan for the two-week winter holiday, and
        put the wheels in motion for my computer adventure.
      </p>
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug"
      >
        Much clearer is the memory of coding a dancing ASCII figure along with a
        listing from an 1986 issue of Bajtek magazine.
      </p>
      <p
        class="text-xl text-gray-800 font-thin mb-6 md:text-2xl px-8 pt-4 leading-snug"
      >
        But mostly I remember playing games on Spectrum.
      </p>
      <div
        class="inline-block mt-6 w-full px-4 lg:w-1/2 xl:w-1/3"
        v-for="(webProject, index) in WebProjects80s"
        v-bind:key="index"
      >
        <ProjectCard :webProject="webProject" />
      </div>
    </div>
  </div>
</template>

<script>
import ProjectCard from "./ProjectCard";
// import json from '../assets/Decades.json'
//use above for GitHub
import json from '../assets/Decades-Local.json'
export default {
  name: "DecadeIndex",
  components: {
    ProjectCard
  },
  data() {
    return {
      showName: false,
      show: true,
    };
  },
  computed: {
    DecadeTexts() {
      return json.DecadeTexts.map((texts) => {
        return texts.text;
      });
    },
    WebProjects() {
      return json.WebProjects.map((projects) => {
        return projects;
      });
    },
    WebProjects80s: function() {
      return this.WebProjects.filter(WebProject => {
        return WebProject.yearMade <= 1990;
      });
    },
    WebProjects90s: function() {
      return this.WebProjects.filter(WebProject => {
        return WebProject.yearMade > 1990 && WebProject.yearMade <= 2000;
      });
    },
    WebProjects00s: function() {
      return this.WebProjects.filter(WebProject => {
        return WebProject.yearMade > 2000 && WebProject.yearMade <= 2010;
      });
    },
    WebProjects10s: function() {
      return this.WebProjects.filter(WebProject => {
        return WebProject.yearMade > 2010 && WebProject.yearMade < 2020;
      });
    },
    WebProjects20s: function() {
      return this.WebProjects.filter(WebProject => {
        return WebProject.yearMade >= 2020;
      });
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.slide-fade-enter-active {
  transition: all 0.8s cubic-bezier(1, 0.5, 0.8, 1);
}
.slide-fade-leave-active {
  transition: all 0.8s ease;
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
