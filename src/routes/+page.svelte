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
    /* hero gradients */
    .hero-gradient-bg {
        z-index: -1;
    }
    .hero-gradient-bg:before, .hero-gradient-bg:after, .hero-gradient-bg div {
        content: '';
        position: absolute;
        filter: blur(10rem);
        z-index: -1;
        border-radius: 50%;
    }
    .hero-gradient-bg:before {
        width: 40rem;
        height: 40rem;
        top: -20rem;
        left: -20rem;
        background: #ECFEFF;
    }
    .hero-gradient-bg:after {
        width: 25rem;
        height: 25rem;
        top: -12.5rem;
        right: -12.5rem;
        background: #FAE8FF;
    }
    .hero-gradient-bg div {
        width: 15rem;
        height: 15rem;
        top: -7.5rem;
        left: calc(50% - 7.5rem);
        background: #f1fff7;
    }
    /* dark */
    .dark .hero-gradient-bg div {background: #3B0764 !important;}

    /* small screen images */
    @media (max-width: 640px) { 
        .hero-gradient-bg:before {
            width: 30rem;
            height: 30rem;
        }
        .hero-gradient-bg:after {
            width: 15rem;
            height: 15rem;
            right: 0px;
        }
        .hero-gradient-bg div {
            display: none;
        }
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

<!-- test -->
<div class="hero-gradient-bg absolute overflow-hidden w-full h-80 top-0 left-0">
    <div></div>
</div>
<div class="mt-40 px-5 grid gap-24">
    <div class="container mx-auto md:max-w-3xl">
        <div class="text-xl text-slate-700 leading-normal md:leading-relaxed grid gap-3 dark:text-slate-200">
            <p class="text-2xl md:text-3xl">Tim Phillips is a designer from Melbourne.</p>
            <p class="">He’s currently working as a product designer at <a class="underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400" href="">carsales</a>, Australia’s largest online automotive marketplace. He is passionate about the craft involved in making intuitive, cohesive and consistent experiences.</p>
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
                <div class="hero small assembler-web-hero transition-all w-full h-full absolute ml-8 md:m-0 left-0 bottom-[-.5rem] md:top-0 bg-no-repeat bg-contain md:bg-cover bg-center"></div>
                </div>
                <div class="hero-wrap group transition-all h-[20rem] md:h-[24rem] p-4 overflow-hidden bg-slate-50 hover:bg-slate-100 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:hover:bg-slate-700 dark:border-slate-600/50">
                    <HeroInfo 
                    category="Web Design"
                    company="Smiggle"
                    btnText="View Work"
                    btnRoute="/work/smiggle/"
                    btnGrouped
                />
                <div class="hero small smiggle-web-hero transition-all w-full h-full absolute ml-8 md:m-0 left-0 bottom-[-.5rem] md:top-0 bg-no-repeat bg-contain md:bg-cover bg-center"></div>
                </div>
            </div>
        </div>
    </div>
</div>