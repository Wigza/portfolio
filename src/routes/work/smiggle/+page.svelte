<script>
    import Button from "../../../lib/Button.svelte";
    import InfoToggle from "../../../lib/InfoToggle.svelte";
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';
    import '@splidejs/splide/dist/css/themes/splide-default.min.css';

    import smig01 from "../../../lib/assets/smig/slides/smig_slide_01.png";
    import smig02 from "../../../lib/assets/smig/slides/smig_slide_02.png";
    import smig03 from "../../../lib/assets/smig/slides/smig_slide_03.png";
    import smig04 from "../../../lib/assets/smig/slides/smig_slide_04.png";
    import smig05 from "../../../lib/assets/smig/slides/smig_slide_05.png";

    let linkStyles = 'underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400';
</script>


<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div class="pb-6 mb-8 border-b border-b-slate-200 dark:border-b-slate-800">
            <div>
                <h1 class="text-4xl font-medium">Smiggle</h1>
                <h5 class="text-xl text-slate-500">Web design team</h5>
            </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-6 gap-8 md:gap-4">
            <div id="info-col" class="md:grid hidden col-span-full md:col-span-2 order-last md:order-first">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">My role</div>
                        <div class="">Web Designer</div>
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
                        <div class="">2017 - 2018</div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Tools</div>
                        <div class="">Adobe Photoshop</div>
                        <div class="">Salesforce</div>
                        <div class="">Adobe Illustrator</div>
                    </div>
                </div>
            </div>
            <div class="col-span-full md:col-span-4">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">About</div>
                        <p>Smiggle is an Australian-based retail chain, that sells vibrant and colourful stationery and related accessories for children. Smiggle is a part of the <a class="{linkStyles}" href="https://www.justgroup.com.au/" target="_blank">Just Group</a>, an Australian company that owns and operates a number of high profile retail chains.</p>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Context</div>
                        <div class="space-y-3">
                            <p>I worked as a Web Designer / Front End Developer on the Smiggle brand for just over 18 months. </p>
                            <p>During my time there I had the opportunity to work on countless digital marketing campaigns across their entire international market base (Australia, New Zealand, UK, Ireland and Asia).</p>
                            <div class="hidden md:block md:mt-4"></div>
                            <InfoToggle />
                            <Button text='View Website' route='https://smiggle.jgl.com.au/' textSize='sm' />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="space-y-10">
        <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
            <div class="space-y-2">
                <h3 class="text-xl font-medium">eCommerce site redesign</h3>
                <p class="text-slate-500">All of the Just Group’s eCommerce sites at the time were split across legacy desktop/mobile sites, rather than a single responsive framework. This created a duplication of work to create/design and build web content across the entire eCommerce team, including Smiggle.</p>
                <p class="text-slate-500">The eCommerce team was working on project to re-platform their tech stack to allow for a responsive, single site for each of the Just Groups brands. As a part of this initiative, the web design team were tasked with re-designing the eCommerce site, which had grown out of date over the years. </p>
                <p class="text-slate-500">I had the opportunity to work on an early concept for the Smiggle site, focusing on some of the core pages: home, product category and product detail.</p>
            </div>
        </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="custom transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <Splide aria-label="My Favorite Images">
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Smiggle category page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={smig01} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Smiggle category page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={smig02} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Smiggle product page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={smig03} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Smiggle home page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={smig04} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Smiggle home page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={smig05} alt=""/>
                            </div>
                        </SplideSlide>
                    </Splide>
                </div>
            </div>
        </div>
    </div>
</div>