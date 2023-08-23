<script>
    import "../app.css";
    import "../global.css";

    import ThemeToggle from "../lib/ThemeToggle.svelte";

    function toggle() {
        let htmlBody = document.querySelector("html");
        htmlBody.classList.toggle("dark");
	}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,300;0,400;0,500;1,300;1,400;1,500&display=swap');
</style>

<nav class="w-full flex items-center justify-between fixed top-0 md:mt-6 md:px-6">
    <!-- sml screen menu -->
    <div class="w-full px-2 pt-4 pb-2 flex justify-between bg-white/75 dark:bg-slate-900/75 backdrop-blur-lg border-slate-200 dark:border-slate-700 border-b shadow shadow-slate-100 dark:shadow-slate-900 md:pt-2 md:w-fit md:justify-normal md:rounded-xl md:border">
        <a class="font-medium text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-50 dark:text-slate-300 dark:hover:bg-white/[.05] hover:text-slate-900 dark:hover:text-slate-50" 
            href="/">
            Tim Phillips, Designer
        </a>
        <a class="text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" 
            href="/about">
            About
        </a>
    </div>
    <div class="hidden md:flex p-1">
        <a class="text-slate-600 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" href="#">Resume</a>
        <a class="text-slate-600 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center" href="https://www.linkedin.com/in/tim-phillips-975239b9/" target="_blank">
            LinkedIn
        </a>
        <ThemeToggle 
            on:click={toggle} 
            classList="text-slate-600 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center"
        />
    </div>
</nav>


<slot />
