<script>
    import Button from "../../../lib/Button.svelte";
</script>

<style>
    .cs-hero-01 {background-image: url($lib/assets/cs/cs-dealbuilder-01.png);}
    .cs-hero-02 {background-image: url($lib/assets/cs/cs-dealbuilder-02.png);}
    .cs-hero-03 {background-image: url($lib/assets/cs/cs-dealbuilder-03.png);}
    .cs-hero-04 {background-image: url($lib/assets/cs/cs-dealbuilder-04.png);}
    .cs-hero-05 {background-image: url($lib/assets/cs/cs-testdrive-01.png);}
    .cs-hero-06 {background-image: url($lib/assets/cs/cs-testdrive-02.png);}
</style>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div class="pb-6 mb-8 border-b border-b-slate-100 dark:border-b-slate-800">
            <div>
                <h1 class="text-4xl font-medium">Carsales</h1>
                <h5 class="text-xl">Digital Retailing</h5>
            </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-6 gap-4">
            <div class="col-span-2 order-last md:order-first">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">My role</div>
                        <div class="">Product Designer</div>
                    </div>
                    <div class="space-y-2">
                        <div class="text-slate-400 text-sm uppercase">Team</div>
                        <div>
                            <div class="">Ahmed Khalid</div>
                            <div class="text-slate-400 text-sm italic">Senior Product Manager</div>
                        </div>
                        <div>
                            <div class="">Peter O'Dwyer</div>
                            <div class="text-slate-400 text-sm italic">Lead Product Designer</div>
                        </div>
                        <div>
                            <div class="">Brendan Hall</div>
                            <div class="text-slate-400 text-sm italic">GM eCommerce</div>
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
            <div class="col-span-4">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">About</div>
                        <p>Carsales is Australia’s largest online automative marketplace (Cars, Motorbikes, Boats etc) that attracts millions of daily users. </p>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Context</div>
                        <div class="space-y-3">
                            <p>I joined Carsales in November 2021, into their newly formed SELECT product team (now Digital Retailing). Our SELECT’s vision was to enable users to buy used cars completely online.</p>
                            <p>My time within this team has given me the opportunity to work across many aspects of Carsales consumer facing product ecosystem. </p>
                            <div class="hidden md:block md:mt-4"></div>
                            <Button text='View Website' route='https://www.carsales.com.au/' textSize='sm' />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="transition-all h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <div class="hero cs-hero-01 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
                </div>
            <div class="transition-all h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-02 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="transition-all h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-03 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-contain bg-center"></div>
            </div>
            <div class="transition-all h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-04 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="transition-all h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-05 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
            <div class="transition-all h-[40rem] p-4 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <div class="hero cs-hero-06 transition-all w-full h-full absolute left-0 top-0 bg-no-repeat bg-cover bg-center"></div>
            </div>
        </div>
    </div>
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div>
            <p class="text-lg font-medium">Thanks for making it this far!</p>
            <p>If you're interested in viewing of some of my other work, check out the links below.</p>
            <div class="mt-4">
                <Button text='Assembler' route='/work/assembler/' textSize='sm' />
                <Button text='PwC Australia' route='/work/assembler/' textSize='sm' />
            </div>
        </div>
    </div>
</div> 