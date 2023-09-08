<script>
    import Button from "../../../lib/Button.svelte";
    import InfoToggle from "../../../lib/InfoToggle.svelte";
    import MoreWork from "../../../lib/MoreWork.svelte";
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';
    let linkStyles = 'underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400';

    import pwcAE01 from "../../../lib/assets/pwc/slides/pwc_ae_slide_01.png";
    import pwcAE02 from "../../../lib/assets/pwc/slides/pwc_ae_slide_02.png";
    import pwcAE03 from "../../../lib/assets/pwc/slides/pwc_ae_slide_03.png";
    import pwcAE04 from "../../../lib/assets/pwc/slides/pwc_ae_slide_04.png";
    
    import '@splidejs/splide/dist/css/themes/splide-default.min.css';
</script>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div class="pb-6 mb-8 border-b border-b-slate-200 dark:border-b-slate-800">
            <div>
                <h1 class="text-4xl font-medium">PwC Australia</h1>
                <h5 class="text-xl text-slate-500">New Ventures</h5>
            </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-6 gap-8 md:gap-4">
            <div id="info-col" class="md:grid hidden col-span-full md:col-span-2 order-last md:order-first">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">My role</div>
                        <div class="">Lead product designer</div>
                    </div>
                    <div class="space-y-2">
                        <div class="text-slate-400 text-sm uppercase">Team</div>
                        <div>
                            <div class="">Thomas Broomfield</div>
                            <div class="text-slate-400 text-sm italic">Senior manager</div>
                        </div>
                        <div>
                            <div class="">Mark Rebeiro</div>
                            <div class="text-slate-400 text-sm italic">Senior Manager</div>
                        </div>
                        <div>
                            <div class="">Megan Linton</div>
                            <div class="text-slate-400 text-sm italic">Senior Manager</div>
                        </div>
                        <div>
                            <div class="">Bridget Connally</div>
                            <div class="text-slate-400 text-sm italic">Senior Consultant</div>
                        </div>
                        <div>
                            <div class="">Daintree Peters</div>
                            <div class="text-slate-400 text-sm italic">Director</div>
                        </div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Timeline</div>
                        <div class="">2018 - 2020</div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Tools</div>
                        <div class="">Sketch</div>
                        <div class="">VS Code</div>
                    </div>
                </div>
            </div>
            <div class="col-span-full md:col-span-4">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">About</div>
                        <p>PwC Australia at the time I joined in 2018, was actively involed in growing their New Ventures capability. New Ventures was an internal innovation unit within PwC, focused on building technology that solved complex problems within PwC's industrial landscape.</p>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Context</div>
                        <div class="space-y-3">
                            <p>I was involved with the <a class="{linkStyles}" href="https://www.pwc.com.au/services/new-ventures/pwc-automation-engine.pdf" target="_blank">Automation Engine</a> (AE) product (which would later become <a class="{linkStyles}" href="/work/assembler/">Assembler</a>), a platform that enabled internal teams to automate complex, often manual processes/tasks and transform them into web applications.</p>
                            <p>I worked as the product designer and supported the engineering team with front end development, I created the design system for both the AE platform and the applications that we built on top of AE.</p>
                            <div class="mt-4"></div>
                            <InfoToggle />
                            <Button text='View Website' route='https://www.pwc.com/gx/en/about/new-ventures.html' textSize='sm' />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="space-y-10">
        <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
            <div class="space-y-2">
                <h3 class="text-xl font-medium">Automation Engine Platofrm</h3>
                <p class="text-slate-500">Dashboard is the DevOps management platform that simplifies the process of setting up web applications, managing the environments they exist within and the maintenance involved with each of the resources within these environments such as databases, user lists and authentication and servers.</p>
            </div>
        </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <Splide aria-label="My Favorite Images">
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Application dashboard</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={pwcAE01} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Global sidebar menu</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={pwcAE02} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Record overview</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={pwcAE03} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Automation manager</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={pwcAE04} alt=""/>
                            </div>
                        </SplideSlide>
                    </Splide>
                </div>
            </div>
        </div>
        <MoreWork />
    </div>
</div>