<script>
    import Button from "../lib/Button.svelte";
    import HeroInfo from "../lib/HeroInfo.svelte";
</script>

<style>
    .cs-hero {
        background-image: url($lib/assets/cs-hero-cover-lrge.png);
    }
    .hero-wrap:hover .hero {
        transform:scale(1.025);
    }
</style>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl">
        <div class="text-2xl text-slate-700 leading-relaxed grid gap-3 md:text-xl dark:text-slate-200">
            <p class="">Tim Phillips is a designer <span>✏️</span> & front-end developer <span>👨‍💻</span> from Melbourne.</p>
            <p class="">He’s currently working as a product designer at <a class="underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400" href="">carsales</a>, Australia’s largest online automotive marketplace.</p>
            <p class="">Find out more about Tim <a class="underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400" href="/about">here</a>.</p>
        </div>
    </div>
    <div class="container mx-auto md:max-w-5xl">
        <div class="hero-wrap group transition-all h-[48rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
            <HeroInfo 
                category="Product Design"
                company="Carsales"
                btnText="View Work"
                btnRoute="/work/carsales/"
                btnGrouped
            />
            <div class="hero cs-hero transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
        </div>
    </div>
    <div class="container mx-auto md:max-w-3xl">
        <div class="text-2xl text-slate-700 leading-relaxed md:text-lg dark:text-slate-200">
            <p class="">Tim Phillips is a designer & front-end developer from Melbourne. He’s currently working as a product designer at carsales, Australia’s largest online automotive marketplace.</p>
            <p class="hidden pt-4 md:block">He is passionate about the craft involved in making intuitive, cohesive and consistent experiences. He also advocates for the role <span class="font-medium">design</span> plays to <span class="font-medium">solve</span> complex <span class="font-medium">problems</span>. </p>
        </div>
    </div>
</div>