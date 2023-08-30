<script>
    import Button from "../../../lib/Button.svelte";
    import { Splide, SplideSlide } from '@splidejs/svelte-splide';

    import testImage01 from "../../../lib/assets/as/slides/builder_slide_test.png";
    import testImage02 from "../../../lib/assets/as/slides/dashboard_slide_test.png";

    import '@splidejs/splide/dist/css/themes/splide-default.min.css';
</script>

<style>

</style>

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
                            <div class="">Thomas Broomfiled</div>
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
    <div class="container mx-auto md:max-w-3xl text-slate-700 dark:text-slate-200">
        <div class="space-y-2">
            <h3 class="text-xl font-medium">Dashboard</h3>
            <p>Dashboard is the DevOps management platform that simplifies the process of setting up web applications, managing the environments they exist within and the maintenance involved with each of the resources within these environments such as databases, user lists and authentication and servers.</p>
        </div>
    </div>
    <div class="container mx-auto md:max-w-5xl">
        <div class="grid gap-10">
            <div class="transition-all py-8 overflow-hidden bg-slate-50 border border-slate-300/50 rounded-lg relative dark:bg-slate-800 dark:border-slate-600/50">
                <Splide aria-label="My Favorite Images">
                    <SplideSlide>
                        <div class="text-slate-500 text-center">
                            <div class="text-sm pb-2">Landing page</div>
                            <img class="w-4/5 mx-auto" src={testImage01} alt=""/>
                        </div>
                    </SplideSlide>
                    <SplideSlide>
                        <div class="text-slate-500 text-center">
                            <div class="pb-2">Another page page</div>
                            <img class="w-4/5 mx-auto" src={testImage02} alt=""/>
                        </div>
                    </SplideSlide>
                </Splide>
            </div>
        </div>
    </div>
</div>