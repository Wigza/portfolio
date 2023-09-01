<script>
    import Button from "../lib/Button.svelte";
    import HeroInfo from "../lib/HeroInfo.svelte";
</script>

<style>
    /* large screen images */
    .cs-hero {
        background-image: url($lib/assets/cs-hero-cover-lrge.png);
    }
    .as-hero {
        background-image: url($lib/assets/as-hero-cover-lrge.png);
    }
    .pwc-hero {
        background-image: url($lib/assets/pwc-hero-cover-lrge.png);
    }
    .assembler-web-hero {
        background-image: url($lib/assets/as-web-cover.png);
    }
    .smiggle-web-hero {
        background-image: url($lib/assets/smg-web-cover.png);
    }
    /* small screen images */
    @media (max-width: 640px) { 
        .cs-hero {
            background-image: url($lib/assets/cs-hero-cover-sml.png);
        }
        .as-hero {
            background-image: url($lib/assets/as-hero-cover-sml.png);
        }
        .pwc-hero {
            background-image: url($lib/assets/pwc-hero-cover-sml.png);
        }
        .hero-wrap .hero.small {
            transform:scale(1.2);
        }
    }

    .hero-wrap:hover .hero {
        transform:scale(1.025);
    }
</style>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl">
        <div class="text-2xl text-slate-700 leading-normal md:leading-relaxed grid gap-3 md:text-xl dark:text-slate-200">
            <p class="">Tim Phillips is a designer <span>✏️</span> & front-end developer <span>👨‍💻</span> from Melbourne.</p>
            <p class="">He’s currently working as a product designer at <a class="underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400" href="">carsales</a>, Australia’s largest online automotive marketplace.</p>
            <p class="">Find out more about Tim <a class="underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400" href="/about">here</a>.</p>
        </div>
    </div>
    <div class="container mx-auto md:max-w-5xl">
        <div class="grid gap-10">
            <div class="hero-wrap group transition-all h-[38rem] md:h-[48rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
                <HeroInfo 
                    category="Product Design"
                    company="Carsales"
                    btnText="View Work"
                    btnRoute="/work/carsales/"
                    btnGrouped
                />
                <div class="hero cs-hero transition-all w-full h-full absolute mt-12 md:mt-0 left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="hero-wrap group transition-all h-[32rem] md:h-[48rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
                <HeroInfo 
                    category="Product Design"
                    company="Assembler"
                    btnText="View Work"
                    btnRoute="/work/assembler/"
                    btnGrouped
                />
                <div class="hero as-hero transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="hero-wrap group transition-all h-[32rem] md:h-[48rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
                <HeroInfo 
                    category="Product Design"
                    company="PwC Australia"
                    btnText="View Work"
                    btnRoute="/work/pwc/"
                    btnGrouped
                />
                <div class="hero pwc-hero transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="grid gap-5 md:grid-cols-2">
                <div class="hero-wrap group transition-all h-[20rem] md:h-[24rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
                    <HeroInfo 
                    category="Web Design"
                    company="Assembler"
                    btnText="View Work"
                    btnRoute="/work/assembler/"
                    btnGrouped
                />
                <div class="hero small assembler-web-hero transition-all w-full h-full absolute ml-8 md:m-0 left-0 top-0 bg-no-repeat bg-contain md:bg-cover bg-center"></div>
                </div>
                <div class="hero-wrap group transition-all h-[20rem] md:h-[24rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
                    <HeroInfo 
                    category="Web Design"
                    company="Smiggle"
                    btnText="View Work"
                    btnRoute="/work/assembler/"
                    btnGrouped
                />
                <div class="hero small smiggle-web-hero transition-all w-full h-full absolute ml-8 md:m-0 left-0 top-0 bg-no-repeat bg-contain md:bg-cover bg-center"></div>
                </div>
            </div>
        </div>
    </div>
</div>