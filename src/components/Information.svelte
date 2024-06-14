svelte
<script>
	import SectionWrapper from "./SectionWrapper.svelte";
    import { fade } from 'svelte/transition';

    function redirectToGitHub(){
        window.location.href="https://github.com/keathkeather"
    }
    function redirectToLinkedin(){
        window.location.href="https://www.linkedin.com/in/keath-ian-lavador-745401232"
    }
</script>

<SectionWrapper id="Information">
    <div class="element" in:fade={{ duration: 1000 }} out:fade={{ duration: 1000 }}>
        <div class="flex flex-col gap-5 sm:gap-5 md:gap-5 flex-1 justify-center pb-10 md:pb-14 mt-96">
            <h1 class="text-mainFontColor ms-auto text-justify">
                 An <span class="text-primaryGreen font-bold">Information Technology</span> Student from Cebu Insitute of Technology,<br/>A Fullstack Developer that aims to bring solutions to your problems 
            </h1>
            <div class="flex flex-row items-center gap-10">
                <a href="../../Keath Ian-Resume.pdf" download="Keath Ian-Resume.pdf" class="button ms-auto flex flex-col">
                    Download Resume
                </a>
                <div class="group relative">
                    <button on:click={redirectToGitHub}>
                        <svg stroke-linejoin="round" stroke-linecap="round" stroke-width="2" stroke="#EEE7DC" fill="none" viewBox="0 0 24 24" class="mt-1 w-8 hover:scale-125 duration-200 hover:mainFontColor"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg>
                    </button>
                    <span class="absolute -top-14 left-[50%] -translate-x-[50%] z-20 origin-left scale-0 px-3">GitHub</span>
                </div>
                <div class="linked group">
                    <button on:click={redirectToLinkedin} class="group flex justify-center p-2 rounded-md bg-mainFontColor hover:scale-125 duration-200 hover:mainFontColor">
                        <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1.1em" viewBox="0 0 512 512" stroke-width="0" fill="currentColor" stroke="currentColor" class="w-5 h-5">
                            <path d="M444.17 32H70.28C49.85 32 32 46.7 32 66.89v374.72C32 461.91 49.85 480 70.28 480h373.78c20.54 0 35.94-18.21 35.94-38.39V66.89C480.12 46.7 464.6 32 444.17 32zm-273.3 373.43h-64.18V205.88h64.18zM141 175.54h-.46c-20.54 0-33.84-15.29-33.84-34.43 0-19.49 13.65-34.42 34.65-34.42s33.85 14.82 34.31 34.42c-.01 19.14-13.31 34.43-34.66 34.43zm264.43 229.89h-64.18V296.32c0-26.14-9.34-44-32.56-44-17.74 0-28.24 12-32.91 23.69-1.75 4.2-2.22 9.92-2.22 15.76v113.66h-64.18V205.88h64.18v27.77c9.34-13.3 23.93-32.44 57.88-32.44 42.13 0 74 27.77 74 87.64z"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
    </div>
</SectionWrapper>