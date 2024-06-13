<script>
	import { Canvas } from "@threlte/core";
	import Contact from "../components/Contact.svelte";
	import Experience from "../components/Experience.svelte";
  import Hero from "../components/Hero.svelte";
	import Information from "../components/Information.svelte";
  import Navigation from "../components/Navigation.svelte";
	import Projects from "../components/Projects.svelte";
	import Scene from "../components/Scene.svelte";
	import Footer from "../components/Footer.svelte";
  
</script>
<style>
  :global(body, html) {
    margin: 0;
    padding: 0;
    overflow: hidden; /* Prevents scrolling */
  }
  
  .scene-container {
    position: fixed; /* or 'absolute' */
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    z-index: -1; /* Ensures it's behind other content */
    opacity: 0.5;
  }

  .content {
    position: relative;
    z-index: 1; /* Ensures content is above the scene */
    /* Additional styling to ensure content is visible and well-positioned */
  }
</style>

<div class=" text-mainFontColor opacity-20 text-sm">Hello try click+dragging/scrolling outside the border</div>
<div class="border border-mainFontColor p-8 max-w-screen-3xl  mx-auto">
  
    <div class="scene-container">
       <Canvas>
        <Scene/>
       </Canvas>
    </div>
    <div class="content">
      <Navigation />
    <main class="">
      <Hero/>
      <Information/>
      <Experience/>
      <Projects/>
      <Contact/>
    </main>
    </div>
</div>


