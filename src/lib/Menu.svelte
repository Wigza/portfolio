<script>
    import ThemeToggle from "./ThemeToggle.svelte";
</script>

<div id="responsive-menu" class="mt-4 h-screen w-full space-y-4">
    <a class="px-3 flex text-lg text-slate-700 dark:text-slate-300" href="/about/">About</a>
    <a class="px-3 flex text-lg text-slate-700 dark:text-slate-300" href="/" >Resume</a>
    <a class="px-3 flex text-lg text-slate-700 dark:text-slate-300" href="https://www.linkedin.com/in/tim-phillips-975239b9/" target="_blank" >LinkedIn</a>
    <ThemeToggle
        classList="transition-all text-lg text-slate-900/50 px-3 py-0.5 rounded-lg hover:bg-slate-500/10 hover:text-slate-900 dark:text-slate-300 dark:hover:bg-white/[.05] dark:hover:text-slate-50 flex items-center"
    />
</div>