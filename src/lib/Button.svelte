<script>
    export let text;
    export let textSize = 'sm';
    export let route;
    export let grouped
</script>

{#if grouped}
    <a class="inline-flex justify-center transition-all px-4 py-2 font-medium text-{textSize} text-slate-600 bg-white/90 backdrop-blur-lg border border-slate-200 rounded-lg drop-shadow-sm group-hover:bg-white group-hover:text-slate-800 group-hover:border-slate-300 group-hover:drop-shadow-md dark:bg-slate-700 dark:border-slate-400 dark:text-slate-200 dark:group-hover:bg-slate-900 dark:group-hover:border-slate-200 dark:group-hover:text-white" href="{route}">
        {text}  
    </a>
{:else}
    <a class="inline-flex justify-center transition-all px-4 py-2 font-medium text-{textSize} text-slate-600 bg-white/90 backdrop-blur-lg border border-slate-200 rounded-lg drop-shadow-sm hover:bg-white hover:text-slate-800 hover:border-slate-300 hover:drop-shadow-md dark:bg-slate-700 dark:border-slate-400 dark:text-slate-200 dark:hover:bg-slate-900 dark:hover:border-slate-200 dark:hover:text-white" href="{route}">
        {text}  
    </a>
{/if} 
