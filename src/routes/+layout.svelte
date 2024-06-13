<script>
  import { onMount } from 'svelte';
  import "../app.css";
  import Footer from "../components/Footer.svelte";
  import Loader from "../components/Loader.svelte";
  
  let isPageLoaded = false;

  onMount(async () => {
    // Simulate delay for loading content
    await new Promise(r => setTimeout(r, 2000));
    isPageLoaded = true;
  });
</script>

{#if !isPageLoaded}
  <Loader />
{:else}
  <div class="fade">
    <slot />
    <Footer />
  </div>
{/if}
