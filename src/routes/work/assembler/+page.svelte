<script>
    import Button from "../../../lib/Button.svelte";
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';

    import asDash01 from "../../../lib/assets/as/slides/dashboard_slide_01.png";
    import asDash02 from "../../../lib/assets/as/slides/dashboard_slide_02.png";
    import asDash03 from "../../../lib/assets/as/slides/dashboard_slide_03.png";
    import asDash04 from "../../../lib/assets/as/slides/dashboard_slide_04.png";
    
    import asApp01 from "../../../lib/assets/as/slides/app_slide_01.png";
    import asApp02 from "../../../lib/assets/as/slides/app_slide_02.png";
    import asApp03 from "../../../lib/assets/as/slides/app_slide_03.png";
    import asApp04 from "../../../lib/assets/as/slides/app_slide_04.png";

    import asWeb01 from "../../../lib/assets/as/slides/web_slide_01.png";
    import asWeb02 from "../../../lib/assets/as/slides/web_slide_02.png";
    import asWeb03 from "../../../lib/assets/as/slides/web_slide_03.png";
    
    import asBuilder01 from "../../../lib/assets/as/slides/builder_slide_01.png";
    import asBuilder02 from "../../../lib/assets/as/slides/builder_slide_02.png";
    import asBuilder03 from "../../../lib/assets/as/slides/builder_slide_03.png";
    import asBuilder04 from "../../../lib/assets/as/slides/builder_slide_04.png";
    import asBuilder05 from "../../../lib/assets/as/slides/builder_slide_05.png";
    import asBuilder06 from "../../../lib/assets/as/slides/builder_slide_06.png";

    import '@splidejs/splide/dist/css/themes/splide-default.min.css';
</script>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div class="pb-6 mb-8 border-b border-b-slate-100 dark:border-b-slate-800">
            <div>
                <h1 class="text-4xl font-medium">Assembler</h1>
            </div>
        </div>
        <div class="grid grid-cols-6 gap-4">
            <div class="col-span-2">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">My role</div>
                        <div class="">Product Designer</div>
                    </div>
                    <div class="space-y-2">
                        <div class="text-slate-400 text-sm uppercase">Team</div>
                        <div>
                            <div class="">Thomas Broomfield</div>
                            <div class="text-slate-400 text-sm italic">CTO</div>
                        </div>
                        <div>
                            <div class="">Daintree Peters</div>
                            <div class="text-slate-400 text-sm italic">CEO</div>
                        </div>
                        <div>
                            <div class="">Mark Rebeiro</div>
                            <div class="text-slate-400 text-sm italic">Solutions Lead</div>
                        </div>
                        <div>
                            <div class="">Megan Linton</div>
                            <div class="text-slate-400 text-sm italic">Product Lead</div>
                        </div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Timeline</div>
                        <div class="">2020 - 2021</div>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Tools</div>
                        <div class="">Sketch</div>
                        <div class="">Figma</div>
                        <div class="">VS Code</div>
                    </div>
                </div>
            </div>
            <div class="col-span-4">
                <div class="grid gap-6">
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">About</div>
                        <p>Assembler is a platform that allows users to build, automate, manage, and scale web applications.</p>
                        <p>It is made up of 3 seperate platforms that work in combination to provide users the necessary tools to digitise their business.</p>
                    </div>
                    <div>
                        <div class="text-slate-400 text-sm uppercase mb-2">Context</div>
                        <div class="space-y-3">
                            <p>I worked as the lead product designer and front end developer at Assembler, within their platform team, where I distributed my efforts across the entire spectrum of their product suite.</p>
                            <p>I was a part of the company from it’s inception, and got to wear many hats during my time their. A few achievements I’m particularly proud of are:</p>
                            <ul class="list-disc list-outside marker:text-slate-300">
                                <li>Lead the design across Assemblers three platforms</li>
                                <li>Design and build their first design system</li>
                                <li>Build the majority front-end of the platform (Svelte, Ruby, Tailwind CSS)</li>
                                <li>Design their marketing website</li>
                                <li>Create their branding</li>
                            </ul>
                            <div class="mt-4"></div>
                            <Button text='View Website' route='https://www.carsales.com.au/' textSize='sm' />
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <div class="space-y-10">
        <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
            <div class="space-y-2">
                <h3 class="text-xl font-medium">Dashboard</h3>
                <p class="text-slate-500">Dashboard is the DevOps management platform that simplifies the process of setting up web applications, managing the environments they exist within and the maintenance involved with each of the resources within these environments such as databases, user lists and authentication and servers.</p>
            </div>
        </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <Splide aria-label="My Favorite Images">
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Application overview</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asDash01} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Landing page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asDash02} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Application environment overview</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asDash03} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Environment user management</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asDash04} alt=""/>
                            </div>
                        </SplideSlide>
                    </Splide>
                </div>
            </div>
        </div>
    </div>
    <div class="space-y-10">
        <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
            <div class="space-y-2">
                <h3 class="text-xl font-medium">Builder</h3>
                <p class="text-slate-500">Builder is the core platform that users interact with to create web pages within their application, set up functional requirements and manage the users within their application.</p>
            </div>
        </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <Splide aria-label="My Favorite Images">
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Admin</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asBuilder01} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Application permissions</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asBuilder02} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Form builder</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asBuilder03} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Page builder</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asBuilder04} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Automations | Create trigger </div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asBuilder05} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Form flow | Create form flow section</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asBuilder06} alt=""/>
                            </div>
                        </SplideSlide>
                    </Splide>
                </div>
            </div>
        </div>
    </div>
    <div class="space-y-10">
        <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
            <div class="space-y-2">
                <h3 class="text-xl font-medium">User facing application</h3>
                <p class="text-slate-500">Theses are the <span class="italic">user facing applications</span> that are built through the previously mentioned platforms (Buildler and Dashboard).</p>
                <p class="text-slate-500">All applications came with a base UI 'theme' that enabled users to build pages and interfaces within the Builder platform by default. Careful consideration was taken into the various components and page layouts that are available to users within this default application.</p>
            </div>
        </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <Splide aria-label="My Favorite Images">
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Application landing page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asApp01} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Dashboard overview</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asApp02} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Form and worklfow</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asApp03} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">User authentication</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asApp04} alt=""/>
                            </div>
                        </SplideSlide>
                    </Splide>
                </div>
            </div>
        </div>
    </div>
    <div id="#marketing" class="space-y-10">
        <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
            <div class="space-y-2">
                <h3 class="text-xl font-medium">Marketing Website</h3>
                <p class="text-slate-500">Assembler needed a web presence after we exited from PwC. This gave me an opportunity to design and build the marketing website. This was a really fun side project ot work on for the team, I collaborated with the entire team to get aligned on the creative direction, tonal voice and strategic positioning of how Assembler could benefit our target market audience.</p>
            </div>
        </div>
        <div class="container mx-auto md:max-w-5xl">
            <div class="grid gap-10">
                <div class="custom transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                    <Splide aria-label="My Favorite Images">
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="text-sm pb-2">Application landing page</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asWeb01} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Dashboard overview</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asWeb02} alt=""/>
                            </div>
                        </SplideSlide>
                        <SplideSlide>
                            <div class="text-slate-500 text-center cursor-grab">
                                <div class="pb-2">Form and worklfow</div>
                                <img class="w-[95%] md:w-11/12 mx-auto" src={asWeb03} alt=""/>
                            </div>
                        </SplideSlide>
                    </Splide>
                </div>
            </div>
        </div>
    </div>
</div>