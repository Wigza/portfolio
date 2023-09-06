<script>
    import "../app.css";
    import "../global.css";
    import { page } from '$app/stores';
    import ThemeToggle from "../lib/ThemeToggle.svelte";
    import MenuToggle from "../lib/MenuToggle.svelte";
    // import GradientBlur from "../lib/GradientBlur.svelte";
    import Menu from "../lib/Menu.svelte";
    import resume from "../lib/assets/TimPhillips_Resume.pdf";

    import pwcBG from "../lib/assets/dropdown/pwc-bg-img.png"
    import asBG from "../lib/assets/dropdown/as-bg-img.png"
    import csBG from "../lib/assets/dropdown/cs-bg-img.png"

    function toggleDropdown() {
        let btn = document.getElementById("work-btn");
        let dropdownMenu = btn.querySelector("#dropdown-menu");

        btn.classList.toggle("active");
        dropdownMenu.classList.toggle("hidden")

    }
 
    function bgChange() {
        let bgCol = document.getElementById("highlight-col");
        let menuItem = this;

        if (menuItem.classList.contains('cs')) {
            // carsales
            bgCol.classList.toggle('carsalesBG');
        } else if (menuItem.classList.contains('pwc')) {
            // pwc
            bgCol.classList.toggle('pwcBG')
        } else if (menuItem.classList.contains('as')) {
            // assembler
            bgCol.classList.toggle('assemblerBG')
        } else {

        }
    }

    let currentRoute = $page.url.pathname;
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
            <a class="transition-all hidden md:inline-flex text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" 
                href="/about">
                About
            </a>
            <button on:click={toggleDropdown} id="work-btn" class="transition-all cursor-pointer relative hidden md:inline-block text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50">
                <div class="flex items-center space-x-1"> 
                    <div>Work</div>
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="w-5 h-5">
                        <path fill-rule="evenodd" d="M5.23 7.21a.75.75 0 011.06.02L10 11.168l3.71-3.938a.75.75 0 111.08 1.04l-4.25 4.5a.75.75 0 01-1.08 0l-4.25-4.5a.75.75 0 01.02-1.06z" clip-rule="evenodd" />
                    </svg>
                </div>
                <div id="dropdown-menu" class="hidden absolute inset-x-0 mt-4 overflow-hidden min-w-[14rem] rounded-xl bg-white dark:bg-slate-900/75 border border-slate-200 dark:border-slate-600 shadow shadow-slate-900/05 dark:shadow-slate-950">
                    <div class="grid grid-cols-5">
                        <div id="highlight-col" class="highlight h-full overflow-hidden col-span-1 transition-all relative">
                            <img src="{csBG}" class="hidden csBG trans-img absolute mix-blend-multiply top-0 right-0" alt="pwc">
                            <img src="{asBG}" class="hidden asBG trans-img absolute mix-blend-multiply top-0 right-0" alt="pwc">
                            <img src="{pwcBG}" class="hidden pwcBG trans-img absolute mix-blend-multiply top-0 right-0" alt="pwc">
                            <div class="absolute h-full w-px bg-slate-900/20 top-0 right-0"></div>
                        </div>
                        <div class="p-2 space-y-px col-span-4">
                            <a on:mouseout={bgChange} on:mouseover={bgChange} class:active="{currentRoute.includes("carsales")}" class="sublink cs rounded-md transition-all flex text-slate-500 px-3 py-1 hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" 
                                href="/work/carsales/">
                                Carsales
                            </a>
                            <a on:mouseout={bgChange} on:mouseover={bgChange} class:active="{currentRoute.includes("assembler")}" class="sublink as rounded-md transition-all flex text-slate-500 px-3 py-1 hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" 
                                href="/work/assembler/">
                                Assembler
                            </a>
                            <a on:mouseout={bgChange} on:mouseover={bgChange} class:active="{currentRoute.includes("pwc")}" class="sublink pwc rounded-md transition-all flex text-slate-500 px-3 py-1 hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" 
                                href="/work/pwc/">
                                PwC Australia
                            </a>
                        </div>
                    </div>
                </div>                 
            </button>
            <MenuToggle />
        </div>
        <Menu />
    </div>
    <div class="hidden md:flex bg-white/20 border border-white/75 backdrop-blur-lg rounded-xl p-1 dark:bg-slate-900/75 dark:border-slate-900/75">
        
        <a class="transition-all text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50" href="{resume}" target="_blank">Résumé</a>
        <a class="transition-all cursor-alias text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center" href="https://www.linkedin.com/in/tim-phillips-975239b9/" target="_blank">
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
