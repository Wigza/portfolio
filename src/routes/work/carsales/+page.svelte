<script>
    import Button from "../../../lib/Button.svelte";
    import InfoToggle from "../../../lib/InfoToggle.svelte";
    import MoreWork from "../../../lib/MoreWork.svelte";
    let linkStyles = 'underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400';
</script>

<style>
    .cs-hero-01 {background-image: url($lib/assets/cs/cs-dealbuilder-01.png);}
    .cs-hero-02 {background-image: url($lib/assets/cs/cs-dealbuilder-02.png);}
    .cs-hero-03 {background-image: url($lib/assets/cs/cs-dealbuilder-03.png);}
    .cs-hero-04 {background-image: url($lib/assets/cs/cs-dealbuilder-04.png);}
    .cs-hero-05 {background-image: url($lib/assets/cs/cs-testdrive-01.png);}
    .cs-hero-06 {background-image: url($lib/assets/cs/cs-testdrive-02.png);}
    @media (max-width: 640px) { 
        .hero {
            background-size: contain;
            transform: scale(2);
        }
    }
</style>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div class="pb-6 mb-8 border-b border-b-slate-200 dark:border-b-slate-800">
            <div>
                <h1 class="text-4xl font-medium">Carsales</h1>
                <h5 class="text-xl text-slate-500">Digital Retailing</h5>
            </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-6 gap-8 md:gap-4">
            <div id="info-col" class="h-fit md:grid hidden col-span-full md:col-span-2 order-last md:order-first">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">My role</div>
                        <div class="">Product Designer</div>
                    </div>
                    <div class="space-y-2">
                        <div class="text-slate-400 text-sm uppercase">Team</div>
                        <div>
                            <div class="">Senior Product Manager</div>
                            <!-- <div class="text-slate-400 text-sm italic">Senior Product Manager</div> -->
                        </div>
                        <div>
                            <div class="">Lead Product Designer</div>
                            <!-- <div class="text-slate-400 text-sm italic">Lead Product Designer</div> -->
                        </div>
                        <div>
                            <div class="">GM eCommerce</div>
                            <!-- <div class="text-slate-400 text-sm italic">GM eCommerce</div> -->
                        </div>
                        <div>
                            <div class="">Content Designer</div>
                            <!-- <div class="text-slate-400 text-sm italic">Senior Product Manager</div> -->
                        </div>
                        <div>
                            <div class="">Head of Research</div>
                            <!-- <div class="text-slate-400 text-sm italic">Senior Product Manager</div> -->
                        </div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Timeline</div>
                        <div class="">2021 - Present</div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Tools</div>
                        <div class="">Figma</div>
                        <div class="">Miro</div>
                        <div class="">Dovetail</div>
                    </div>
                </div>
            </div>
            <div class="col-span-full md:col-span-4">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">About</div>
                        <p>Carsales is Australia’s largest online automotive marketplace (Cars, Motorbikes, Boats etc) that attracts millions of daily users. </p>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Context</div>
                        <div class="space-y-3">
                            <p>I joined carsales in November 2021, into their newly formed <a class="{linkStyles}" href="https://www.carsales.com.au/carsales-select/" target="_blank">SELECT</a> product team (now Digital Retailing). Our vision at the time was to ‘enable users to buy used cars completely online’.</p>
                            <p>My time within this team has given me the opportunity to work across many aspects of carsales consumer facing product ecosystem.</p>
                            <p>This has included re-designing elements of the listing detail page, to enable consumers to complete more aspects of the car enquiry process online, through carsales’ platform. Designing an enriched enquiry experience for SELECT vehicles. Creating carsales’ first online finance application process. Most recently I’ve been exploring how to give consumers the ability to book test drives on dealer listings.</p>
                            <div class="hidden md:block md:mt-4"></div>
                            <InfoToggle />
                            <Button text='View Website' route='https://www.carsales.com.au/' textSize='sm' />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="transition-all h-[24rem] md:h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <div class="hero cs-hero-01 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
                </div>
            <div class="transition-all h-[24rem] md:h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-02 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="transition-all h-[24rem] md:h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-03 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-contain bg-center"></div>
            </div>
            <div class="transition-all h-[24rem] md:h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-04 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="transition-all h-[24rem] md:h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-05 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="transition-all h-[24rem] md:h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-06 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
        </div>
    </div>
    <MoreWork />
</div> 