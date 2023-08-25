<script>
    import Button from "./Button.svelte";

    export let category;
    export let company;
    export let btnText;
    export let btnRoute;
    export let btnGrouped;
</script>

<div class="flex items-center justify-between w-full relative z-10">
    <div class="flex items-center space-x-2">
        <div class="text-sm text-slate-500 group-hover:text-slate-700 dark:text-slate-300 dark:group-hover:text-white">{company}</div>
        <div class="hidden md:block bg-slate-400 dark:bg-slate-600 dark:group-hover:bg-slate-500 w-1 h-1 rounded-lg"></div>
        <div class="text-sm text-slate-500 group-hover:text-slate-700 dark:text-slate-300 dark:group-hover:text-white hidden md:block">{category}</div>
    </div>
    <div>
        <Button text={btnText} route={btnRoute} grouped={btnGrouped} />
    </div>
</div>