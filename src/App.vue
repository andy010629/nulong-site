<!-- @format -->

<template>
  <div class="flex items-center justify-start">
    <div
      ref="title"
      v-show="vshow_title"
      class="w-full flex justify-center items-center h-screen"
    >
      <div
        class="absolute group duration-1000 z-20"
        :class="{ 'opacity-0': !show_title }"
      >
        <div
          class="absolute -inset-2 bg-gradient-to-r from-red-700 to-blue-700 rounded-lg blur opacity-70 group-hover:opacity-100 transition duration-1000 group-hover:duration-500 animate-tilt"
        ></div>
        <button
          @click="click_title()"
          class="relative px-2 md:px-7 py-4 bg-black rounded-lg leading-none flex items-center divide-x divide-gray-600"
        >
          <div class="flex items-center p-6">
            <span
              class="text-gray-100 text-xl md:text-3xl font-mono font-semibold tracking-widest select-none leading-loose"
            >
              {{ obj.output }}</span
            >
            <span
              class="typed-cursor text-black text-base md:text-base font-mono font-semibold select-none"
              >A</span
            >
          </div>
        </button>
      </div>
    </div>

    <div
      v-show="vshow_content"
      :class="{ 'opacity-0': !content1, '-translate-x-48': !content1 }"
      class="font-mono tracking-wide text-gray-100 duration-1000 p-0 md:p-8 md:ml-60 ml-0"
    >
      <div class="flex items-center justify-center md:justify-start h-screen">
        <div class="flex flex-col justify-center">
          <p class="md:text-6xl text-4xl mb-2">Hi, I'm Nulong</p>
          <!-- <p class="md:text-2xl text-lg">A Student study in CSIE</p> -->
          <p class="md:text-2xl text-lg">Life = Programming + Music</p>
          <div class="flex mt-8 space-x-6">
            <a
              href="https://github.com/andy010629"
              target="_blank"
              class="w-8 h-8 rounded-xl"
            >
              <i
                class="fab fa-github text-4xl opacity-60 hover:opacity-90 duration-500"
              ></i>
            </a>
            <a
              href="https://www.facebook.com/andy010629"
              class="w-8 h-8 rounded-xl"
            >
              <i
                class="fab fa-facebook text-4xl opacity-60 hover:opacity-90 duration-500"
              ></i>
            </a>
            <a
              href="https://www.instagram.com/ives0629/"
              class="w-8 h-8 rounded-xl"
            >
              <i
                class="fab fa-instagram text-4xl opacity-60 hover:opacity-90 duration-500"
              ></i>
            </a>
          </div>
        </div>

        <!-- <span
          class="left-[50%] -translate-x-[50%] absolute hover:translate-y-9 animate-bounce duration-500 select-none bottom-20 material-symbols-outlined text-6xl"
        >
          expand_more
        </span> -->
      </div>

      <div class="flex flex-col w-full mt-48">
        <div class="text-gray-200 mb-8 md:mb-24 md:p-0 p-6">
          <div class="md:text-6xl text-4xl fade-in-left">About Me</div>
          <p class="md:text-2xl text-lg opacity-70 fade-in-left">
            A Student studying in CSIE
          </p>
        </div>

        <div
          class="flex md:space-x-20 flex-col md:flex-row ml-0 md:ml-32 items-center fade-in-bottom"
        >
          <div>
            <img
              class="w-52 h-52 md:w-96 md:h-96 rounded-xl opacity-80"
              src="/avatar.jfif"
              alt=""
            />
          </div>
          <div
            class="text-gray-400 w-80 md:w-96 md:text-2xl text-lg tracking-widest font-bold md:leading-[50px] md:p-0 p-6"
          >
            <div class="mb-6">
              喜歡探索新技術，學習不同領域的知識，並實際應用，改善生活中的問題。
            </div>
            <div>
              習慣以 "目標導向"
              的方式學習，常常看到特別的東西就會不小心栽進去，最後不知不覺就天亮了XD。
            </div>
          </div>
        </div>
      </div>

      <div class="flex flex-col mt-40 md:mt-64">
        <div class="text-gray-200 mb-8 md:mb-24 md:p-0 p-4">
          <div class="md:text-6xl text-4xl fade-in-left">Experiences</div>
        </div>
        <div class="md:ml-16">
          <div class="mb-24 px-6">
            <div class="md:text-4xl text-gray-400 text-2xl mb-8 fade-in-bottom">
              Work Experiences
            </div>
            <div
              class="flex flex-col md:ml-12 text-base md:text-xl fade-in-bottom"
            >
              <div class="">2022</div>
              <div class="ml-4 mb-4 mt-2 flex flex-col space-y-4">
                <div>
                  • GDSC (Google Developers Student Club) Core Team Members
                </div>
              </div>

              <div class="">2020</div>
              <div class="ml-4 mb-4 mt-2 flex flex-col space-y-4">
                <div>• GDSC (Google Developers Student Club) Lead</div>
                <div>• MCUOSC (MingChuang OpenSource Club) Director</div>
                <div>
                  • Teaching Assistant of Computer Programming II - Ming Chuan
                  University
                </div>
              </div>

              <div>2019</div>
              <div class="ml-4">
                <div>
                  • Teaching Assistant of Computer Programming I - Ming Chuan
                  University
                </div>
              </div>
            </div>
          </div>
          <div class="mb-8 px-6">
            <div class="md:text-4xl text-gray-400 text-2xl mb-8 fade-in-bottom">
              Extracurricular Activities
            </div>
            <div
              class="flex flex-col text-base md:text-xl md:ml-12 fade-in-bottom"
            >
              <div>2022</div>
              <div class="ml-4 mb-4 mt-2 flex flex-col space-y-4">
                <div>
                  • GDSC(Google Developers Student Club) Core Team Members
                </div>
              </div>
              <div>2021</div>
              <div class="ml-4 mb-4 mt-2 flex flex-col space-y-4">
                <div>
                  • ICPC-Taiwan National Contest for Private Universities -
                  Silver
                </div>
                <div>• GDSC Northern Region Hackathon Coordinator</div>
                <div>• GDSC North Region Summit Coordinator/Event Planning</div>
              </div>
              <div>2020</div>
              <div class="ml-4 mb-4 mt-2 flex flex-col space-y-4">
                <div>• Collegiate Programming Examination - Rank 1.3%</div>
                <div>
                  • NCPU(ICPC-Taiwan National Contest for Private Universities)
                  - Bronze
                </div>
                <div>
                  • MOS-Hackathon(MingChuang OpenSource Hackathon) Event General
                  Coordinator
                </div>
                <div>
                  • MingChuang HotMusic Club Computer and Information Manager
                </div>
              </div>
              <div>2019</div>
              <div class="ml-4 mb-4 mt-2 flex flex-col space-y-4">
                <div>• MingChuang programming ranking competition - 1st</div>
                <div>
                  • NASA Space Apps Challenge 2019 @ Taipei - Innovation Award
                </div>
                <div>
                  • NASA Space Apps Challenge 2019 @ Taipei - 羽澤光電特別獎
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="flex flex-col mt-40 md:mt-52">
        <div class="text-gray-200 mb-8 md:mb-24 md:p-0 p-4">
          <div class="md:text-5xl mb-20 text-4xl fade-in-left">
            Project Contributions
          </div>
          <div class="fade-in-bottom"><a href="https://up.mcuosc.dev" target="_blank" class="fade-in-bottom">
            <img
              class="w-6/12 rounded-xl hover:scale-110 duration-1000 opacity-80"
              src="https://www.fanlan.net/static/72ca3958d2941b1826561b25d799c40e/d5dc4/demo.webp"
              alt=""
            />
          </a></div>
          
        </div>
      </div>
      <!-- <div class="flex flex-col mt-80">
        <div class="text-gray-200 mb-8 md:mb-24 md:p-0 p-6">
          <div class="md:text-6xl text-4xl">Projects</div>
        </div>
      </div> -->
    </div>
  </div>

  <!-- <div class="fixed top-0 w-full z-50 h-screen bg-yellow-400 text-white">123</div> -->
</template>

<script>
import EasyTyper from 'easy-typer-js'
export default {
  name: 'App',
  data() {
    return {
      obj: {
        output: '',
        isEnd: false,
        speed: 150,
        singleBack: false,
        sleep: 0,
        type: 'normal',
        backSpeed: 40,
        sentencePause: false,
      },
      show_title: true,
      vshow_title: true,
      vshow_content: false,
      content1: false,
      fadeInElements: [],
      a: [],
    }
  },
  mounted() {
    console.log('onMounted')
    new EasyTyper(this.obj, "Nulong's Website <>")
  },
  methods: {
    click_title() {
      console.log(this.show_title)
      this.show_title = false
      this.a = ['test']

      setTimeout(() => {
        this.vshow_title = false
        this.vshow_content = true
      }, 1000)
      setTimeout(() => {
        this.content1 = true
        this.fadeInElements = Array.from(
          document.getElementsByClassName('fade-in-left')
        ).concat(Array.from(document.getElementsByClassName('fade-in-bottom')))
        document.addEventListener('scroll', this.handleScroll)
        this.handleScroll()
      }, 1300)
    },

    handleScroll() {
      for (var i = 0; i < this.fadeInElements.length; i++) {
        var elem = this.fadeInElements[i]
        if (this.isElemVisible(elem)) {
          elem.style.opacity = '1'
          elem.style.transform = 'translateX(0)'
          elem.style.transform = 'translateY(0)'
          this.fadeInElements.splice(i, 1) // only allow it to run once
        }
      }
    },
    isElemVisible(el) {
      var rect = el.getBoundingClientRect()
      var elemTop = rect.top - 100 // 200 = buffer
      var elemBottom = rect.bottom
      return elemTop < window.innerHeight && elemBottom >= 0
    },
  },
}
</script>

<style>
.fade-in-left {
  opacity: 0;
  transform: translateX(-500px);
  transition: all 1s ease-in-out;
}

.fade-in-bottom {
  opacity: 0;
  transform: translateY(200px);
  transition: all 1s ease-in-out;
}

.typed-cursor {
  border-right: 0.2em solid white; /* The typwriter cursor */
  animation: blink-caret 0.75s step-end infinite;
}
/* The typewriter cursor effect */
@keyframes blink-caret {
  from,
  to {
    border-color: transparent;
  }
  50% {
    border-color: white;
  }
}
</style>