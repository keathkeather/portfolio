<script>
    import { onMount } from 'svelte';
    import scare from '../lib/assets/scare.jpg';
    import joke from '../lib/assets/joke.jpg';
    onMount(() => {
        const a = document.createElement('a');
        a.href = joke; // URL of the file to download
        a.download = 'joke.jpg'; // The filename to download as
        document.body.appendChild(a); // Append to the document
        a.click(); // Programmatically click the anchor to trigger the download
        document.body.removeChild(a); // Clean up
    });
</script>

<div class="flex">
    <img alt="The project logo" src={scare} />
    <div class="text-mainFontColor">
        Congratulations, you have found the easter egg.
        Malicious file is now injected on to your system :)
    </div>
</div>