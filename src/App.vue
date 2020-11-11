<template>
  <div
    class="max-w-4xl flex items-center h-auto lg:h-screen flex-wrap mx-auto my-32 lg:my-0"
  >
    <!--Main Col-->
    <div
      id="profile"
      class="w-full lg:w-3/5 rounded-lg lg:rounded-l-lg lg:rounded-r-none shadow-2xl bg-white opacity-75 mx-6 lg:mx-0"
    >
      <div class="p-4 md:p-12 text-center lg:text-left">
        <!-- Image for mobile view-->
        <div
          class="block lg:hidden rounded-full shadow-xl mx-auto -mt-16 h-48 w-48 bg-cover bg-center"
          style="background-image: url('https://umentalf.sirv.com/profile.jpg')"
        ></div>

        <h1 class="text-3xl font-bold pt-8 lg:pt-0">Senthuran Elangovan</h1>
        <div
          class="mx-auto lg:mx-0 w-4/5 pt-3 border-b-2 border-teal-500 opacity-25"
        ></div>
        <p
          class="pt-4 text-base font-bold flex items-center justify-center lg:justify-start"
        >
          <svg
            class="h-4 fill-current text-teal-700 pr-4"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 20 20"
          >
            <path
              d="M9 12H1v6a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-6h-8v2H9v-2zm0-1H0V5c0-1.1.9-2 2-2h4V2a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v1h4a2 2 0 0 1 2 2v6h-9V9H9v2zm3-8V2H8v1h4z"
            ></path>
          </svg>
          Software Engineer
        </p>

        <p
          class="pt-2 text-xs font-bold lg:text-sm flex items-center justify-center lg:justify-start"
        >
          <svg
            class="h-4 fill-current text-teal-700 pr-4"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 20 20"
          >
            <path
              d="M10 20a10 10 0 1 1 0-20 10 10 0 0 1 0 20zm7.75-8a8.01 8.01 0 0 0 0-4h-3.82a28.81 28.81 0 0 1 0 4h3.82zm-.82 2h-3.22a14.44 14.44 0 0 1-.95 3.51A8.03 8.03 0 0 0 16.93 14zm-8.85-2h3.84a24.61 24.61 0 0 0 0-4H8.08a24.61 24.61 0 0 0 0 4zm.25 2c.41 2.4 1.13 4 1.67 4s1.26-1.6 1.67-4H8.33zm-6.08-2h3.82a28.81 28.81 0 0 1 0-4H2.25a8.01 8.01 0 0 0 0 4zm.82 2a8.03 8.03 0 0 0 4.17 3.51c-.42-.96-.74-2.16-.95-3.51H3.07zm13.86-8a8.03 8.03 0 0 0-4.17-3.51c.42.96.74 2.16.95 3.51h3.22zm-8.6 0h3.34c-.41-2.4-1.13-4-1.67-4S8.74 3.6 8.33 6zM3.07 6h3.22c.2-1.35.53-2.55.95-3.51A8.03 8.03 0 0 0 3.07 6z"
            ></path>
          </svg>
          Colombo, Sri Lanka
        </p>
        <p
          class="pt-8 text-xs font-bold lg:text-sm flex items-center justify-center lg:justify-start"
        >
          Current Stak :
          <span id="sliding-text" class="sliding-words-wrapper">
            <template v-for="(stack, index) in stack" :key="index">
              <span
                class="single-text"
                :class="stack.isShow ? 'is-visible' : 'is-hidden'"
                >{{ stack.name }}</span
              >
            </template>
          </span>
        </p>
        <p class="pt-8 text-sm">
          Based on almost 3 years experience as a software engineer, I am
          excellent at working with others to achieve a certain objective on
          time and with excellence
        </p>

        <div class="pt-12 pb-8">
          <a
            class="bg-teal-700 hover:bg-teal-900 text-white font-bold py-2 px-4 rounded-full"
            href=" https://umentalf.sirv.com/Senthuran%20Elangovan.pdf"
            target="_blank"
          >
            Download CV
          </a>
        </div>

        <div
          class="mt-6 pb-16 lg:pb-0 w-4/5 lg:w-full mx-auto flex items-center"
        >
          <a class="link px-3" href="#"
            ><svg
              class="h-6 fill-current text-gray-600 hover:text-teal-700"
              role="img"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>GitHub</title>
              <path
                d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"
              ></path></svg
          ></a>
          <a class="link px-3" href="#"
            ><svg
              class="h-6 fill-current text-gray-600 hover:text-teal-700"
              role="img"
              viewBox="0 0 24 24"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>GitHub</title>
              <path
                d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"
              ></path></svg
          ></a>
        </div>

        <!-- Use https://simpleicons.org/ to find the svg for your preferred product -->
      </div>
    </div>

    <div class="w-full lg:w-2/5">
      <img
        src="https://umentalf.sirv.com/profile.jpg"
        class="rounded-none lg:rounded-lg shadow-2xl hidden lg:block"
      />
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
  },
  data() {
    return {
      stack: [
        { id: 0, name: "JavaScript Fullstack", isShow: false },
        { id: 1, name: "Vue js (Vue Router/ VUEX)", isShow: false },
        { id: 2, name: "Node js /express", isShow: false },
        { id: 3, name: "MongoDB", isShow: false },
      ],
    };
  },
  mounted() {
    setInterval(() => {
      for (let i = 0; i < this.stack.length; i++) {
        this.setDelay(i);
      }
    }, this.stack.length * 2000);
  },
  methods: {
    setDelay(i) {
      setTimeout(() => {
        if (this.stack[i].id != 0) {
          this.stack[i - 1].isShow = false;
        } else {
          this.stack[this.stack.length - 1].isShow = false;
        }
        this.stack[i].isShow = true;
      }, this.stack[i].id * 2000);
    },
  },
};
</script>

<style scoped>
.sliding-words-wrapper {
  position: relative;
  display: inline-flex;
  flex-direction: column;
  align-items: start;
  justify-content: center;
  vertical-align: top;
  width: 50%;
  overflow: visible;
  text-align: left;
  padding-left: 0.1em;
  padding-top: 1.5em;
}
.sliding-words-wrapper span.single-text {
  position: absolute;
  opacity: 0;
  top: 0.2em;
}
.sliding-words-wrapper span.single-text.is-hidden {
  -webkit-animation: slide-out 0.6s;
  animation: slide-out 0.6s;
}
.sliding-words-wrapper span.single-text.is-visible {
  top: 0;
  opacity: 1;
  -webkit-animation: slide-in 0.6s;
  animation: slide-in 0.6s;
}
@media only screen and (max-width: 330px) {
  .sliding-words-wrapper {
    display: flex;
    padding-left: 0;
  }
}
@-webkit-keyframes slide-in {
  0% {
    opacity: 0;
    -webkit-transform: translateY(-100%);
    transform: translateY(-100%);
  }
  60% {
    opacity: 1;
    -webkit-transform: translateY(20%);
    transform: translateY(20%);
  }
  100% {
    opacity: 1;
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
}
@keyframes slide-in {
  0% {
    opacity: 0;
    -webkit-transform: translateY(-100%);
    transform: translateY(-100%);
  }
  60% {
    opacity: 1;
    -webkit-transform: translateY(20%);
    transform: translateY(20%);
  }
  100% {
    opacity: 1;
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
}
@-webkit-keyframes slide-out {
  0% {
    opacity: 1;
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  60% {
    opacity: 0;
    -webkit-transform: translateY(120%);
    transform: translateY(120%);
  }
  100% {
    opacity: 0;
    -webkit-transform: translateY(100%);
    transform: translateY(100%);
  }
}
@keyframes slide-out {
  0% {
    opacity: 1;
    -webkit-transform: translateY(0);
    transform: translateY(0);
  }
  60% {
    opacity: 0;
    -webkit-transform: translateY(120%);
    transform: translateY(120%);
  }
  100% {
    opacity: 0;
    -webkit-transform: translateY(100%);
    transform: translateY(100%);
  }
}
</style>
