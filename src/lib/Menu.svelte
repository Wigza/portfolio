<script>
    import ThemeToggle from "./ThemeToggle.svelte";
    import resume from "../lib/assets/TimPhillips_Resume.pdf";
    function toggle() {
        let btn = document.getElementById("menu-btn");
        let menu = document.getElementById("responsive-menu");
        let htmlBody = document.querySelector("html");

        btn.classList.toggle("active");
        menu.classList.toggle("active");
        htmlBody.classList.toggle("overflow-hidden")        
	}
</script>

<div id="responsive-menu" class="mt-4 h-screen w-full space-y-4">
    <div class="mx-3 text-slate-400 text-sm uppercase dark:text-slate-400">Work</div>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-300" href="/work/carsales/">Carsales</a>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-300" href="/work/assembler/">Assembler</a>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-300" href="/work/pwc/">PwC Australia</a>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-300" href="/work/smiggle/">Smiggle</a>
    <div class="h-px mx-3 bg-slate-200"></div>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-30" href="/about/">About</a>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-300" target="_blank" href="{resume}" >Resume</a>
    <a on:click={toggle} class="mx-3 flex text-lg text-slate-700 dark:text-slate-300" href="https://www.linkedin.com/in/tim-phillips-975239b9/" target="_blank" >LinkedIn</a>
    <ThemeToggle
        classList="transition-all text-lg text-slate-700/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center"
    />
</div>