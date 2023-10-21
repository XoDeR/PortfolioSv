<script>
  import Step from "./Step.svelte"

  // TODO choose appropriate icons from FontAwesome Icons
  let steps = [
    {name: "BookSeller", icon: "fa-solid fa-cart-shopping"},
    {name: "NetHub", icon: "fa-solid fa-list-check"},
    {name: "HealthProvider", icon: "fa-solid fa-diagram-project"},
  ]
</script>

<main class="flex flex-col flex-1 p-4">
  <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
    <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="montserrat text-violet-400">Victor</span> Codeberg <br/>Full Stack
        <span class="montserrat text-violet-400">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400">favorite tech</span> includes JavaScript (React or NEXT.JS),
        TailwindCSS, Node.js + Express.js, PostgreSQL, MongoDb, Supabase!
      </p>
      <a class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl montserrat relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" href="#" target="_blank">
        <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200">
        </div>
        <h4 class="relative z-9">Get in touch &rarr;</h4>
      </a>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img src={"images/profile-web-developer.jpg"} alt="Profile" class="object-cover z-[2] max-h-[70vh]" />
    </div>
  </section>
  <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-lg sm:text-xl md:text-2xl">
        A few of my creative endeavors.
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="montserrat text-violet-400">see</span> my work?
      </h3>
    </div>
    <a href="https://www.youtube.com/watch?v=fhfdhfjfgj"
      target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex 
      items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
        <i class="fa-regular fa-circle-play"></i>
        <p>Watch the video</p>
    </a>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>BookSeller is a store to sell books created with
        <strong class="text-violet-500">React, Node.js + Express.js, PostgreSQL</strong>
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>NetHub is a Full Stack
        <strong class="text-violet-500">Next.js, Node.js + Express.js & MongoDb</strong>
        Social Network application. 
        </p>
      </Step>
      <Step step={steps[2]}>
        <p>HealthProvider is a</p>
        <strong class="text-violet-500">React, Node.js + Express.js & MongoDb</strong>
         application to book appointments with different doctors in different time slots.
      </Step>
    </div>
  </section>
  <section id="about" class="py-20 pt-10 lg:pt-16 lg-py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
    <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0
      before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700
      after:absolute after:bottom-0
      after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700">
      <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">A bit <span class="montserrat text-violet-500">about</span> me.</h3>
    </div>
    <p class="mx-auto montserrat font-semibold text-lg sm:texl-xl md:text-2xl">I am . . .</p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]"></div>
  </section>
</main>