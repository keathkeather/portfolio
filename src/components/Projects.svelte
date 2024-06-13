<script>
	import SectionWrapper from "./SectionWrapper.svelte";


</script>

<style>
  .projects-container {
      max-height: 600px; /* Adjust based on your needs */
      overflow-y: auto; /* Enables vertical scrolling */
      display: flex;
      flex-direction: column;
      gap: 5px; /* Keeps your existing gap */
      padding-bottom: 10px; /* Keeps your existing padding */
      align-items: end; /* Keeps your existing alignment */
      margin-top: 40px; /* Keeps your existing margin top */
  }
</style>

<SectionWrapper id="Projects">
    <div class="projects-container">
        <div class="flex flex-col gap-5 sm:gap-5 md:gap-5 flex-1   pb-10 md:pb-14 items-end ">
          <div class="notification ,">
            <div class="notiglow"></div>
            <div class="notiborderglow"></div>
            <div class="notititle">Tagatalk</div>
            <div class="notibody">A Mobile Filipino Proficiency App</div>
          </div>
          <div class="notification mt-">
            <div class="notiglow"></div>
            <div class="notiborderglow"></div>
            <div class="notititle">Berdola</div>
            <div class="notibody">Sql Querying ChatBot</div>
          </div>
          <div class="notification ,">
            <div class="notiglow"></div>
            <div class="notiborderglow"></div>
            <div class="notititle">Lit</div>
            <div class="notibody">A Web Based Filipino Proficiency App</div>
          </div>
          <div class="notification">
            <div class="notiglow"></div>
            <div class="notiborderglow"></div>
            <div class="notititle">SimpleSignLanguage</div>
            <div class="notibody">Sign Language Recognition System using Aritifical Intellgence</div>
          </div>
          <div class="notification">
            <div class="notiglow"></div>
            <div class="notiborderglow"></div>
            <div class="notititle">Green8</div>
            <div class="notibody"> Next.js static landing Page for a client</div>
          </div>
          <div class="notification">
            <div class="notiglow"></div>
            <div class="notiborderglow"></div>
            <div class="notititle">SpeakSnap</div>
            <div class="notibody">Language translation app using OCR and Google Translate</div>
          </div>
       </div>
    </div>
</SectionWrapper>