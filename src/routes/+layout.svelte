<script>
    import "../app.css";
    import "../global.css";

    import ThemeToggle from "../lib/ThemeToggle.svelte";
    import MenuToggle from "../lib/MenuToggle.svelte";
    import Menu from "../lib/Menu.svelte";

    import resume from "../lib/assets/TimPhillips_Resume.pdf"

    let year = new Date().getFullYear();
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,300;0,400;0,500;1,300;1,400;1,500&display=swap');
</style>

<!-- global nav -->
<nav class="w-full flex items-center justify-between fixed z-40 top-0 md:mt-6 md:px-6">
    <!-- sml screen menu -->
    <div class="w-full px-2 py-4 md:p-1 bg-white/75 dark:bg-slate-900/75 backdrop-blur-lg border-slate-200 dark:border-slate-600 border-b shadow shadow-slate-900/05 dark:shadow-slate-950 md:w-fit md:justify-normal md:rounded-xl md:border">
        <div class="flex justify-between">
            <a class="transition-all text-lg md:text-base font-medium text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 dark:text-slate-300 dark:hover:bg-white/[.05] hover:text-slate-900 dark:hover:text-slate-50" 
                href="/">
                Tim Phillips, Designer
            </a>
            <MenuToggle />
        </div>
        <Menu />
    </div>
    <div class="hidden md:flex bg-white/20 border border-white/75 backdrop-blur-lg rounded-xl p-1 dark:bg-slate-900/75 dark:border-slate-900/75">
        <a class="transition-all text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" 
            href="/about">
            About
        </a>
        <a class="transition-all text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" href="{resume}" target="_blank">Résumé</a>
        <a class="transition-all text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center" href="https://www.linkedin.com/in/tim-phillips-975239b9/" target="_blank">
            LinkedIn
        </a>
        <ThemeToggle 
            classList="transition-all text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center"
        />
    </div>
</nav>

<slot />

<footer class="mt-24 px-5 pb-8 md:px-0 container mx-auto md:max-w-3xl">
    <div class="text-sm w-full justify-between md:flex items-center">
        <div class="font-medium text-slate-700 dark:text-slate-300">Tim Phillips, Designer</div>
        <div class="text-slate-700 dark:text-slate-300">Designed and built by Tim Phillips, {year}</div>
    </div>
</footer>
