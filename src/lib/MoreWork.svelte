<script>
    import Button from "./Button.svelte";
    import { page } from '$app/stores';
    let currentRoute = $page.url.pathname;
</script>

<div class="container mx-auto md:max-w-3xl">
    <div class="space-y-4">
        <div>
            <h3 class="text-lg font-medium text-slate-800">Thanks for viewing this page :)</h3>
            <p class="text-slate-600">If you’re interested in seeing more examples of my work, find them below.</p>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
            {#if !currentRoute.includes("carsales")}
                <Button 
                    text='Carsales' 
                    route='/work/carsales/' />
            {/if}
            {#if !currentRoute.includes("assembler")}
            <Button 
                text='Assembler' 
                route='/work/assembler/' />
            {/if}
            {#if !currentRoute.includes("pwc")}
            <Button 
                text='PwC Australia' 
                route='/work/pwc/' />
            {/if}
            {#if !currentRoute.includes("smiggle")}
                <Button 
                    text='Smiggle' 
                    route='/work/smiggle/' />
            {/if}
        </div>
    </div>
</div>