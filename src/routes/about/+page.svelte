<script>
    import profile from '../../lib/assets/profile.jpeg';
    let linkStyles = 'underline decoration-teal-400 decoration-2 underline-offset-2 transition-all hover:underline-offset-4 hover:decoration-teal-200 hover:text-teal-400';
    import resume from "../../lib/assets/TimPhillips_Resume.pdf"

    function toggleImage() {
        let image = document.getElementById('toggle-dp');
        image.classList.toggle('hidden')
    }
</script>

<div class="mt-32 px-5 grid gap-20">
    <div class="container mx-auto md:max-w-3xl">
        <div class="text-slate-700 leading-relaxed grid md:grid-cols-4 gap-12 md:gap-6 dark:text-slate-200">
            <div class="relative md:col-span-1 order-last">
                <div class="relative">
                    <img src="{profile}" id='toggle-dp' class="absolute md:relative z-10 w-24 md:w-36 md:mx-auto right-4 md:right-0 top-4 md:top-0 border-4 border-white dark:border-slate-900 shadow-md shadow-slate-900/10 dark:shadow-slate-950/20 rounded-lg" alt="">
                </div>
                <div class="p-4 md:pt-20 md:-mt-20 rounded-lg bg-slate-50 dark:bg-slate-800">
                    <div class="md:mt-4 flex flex-col content-center">
                        <a class="group md:w-full w-3/5 text-slate-700/80 hover:text-slate-900 dark:text-slate-200 items-center justify-between rounded-md transition-all px-2 py-1 flex hover:bg-slate-900/10 dark:hover:bg-slate-700" href="mailto:timphillips1991@gmail.com">
                            Email
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="transition-all group-hover:opacity-100 opacity-0 w-5 h-5">
                                <path fill-rule="evenodd" d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z" clip-rule="evenodd" />
                            </svg>                              
                        </a>
                        <a class="group md:w-full w-3/5 text-slate-700/80 hover:text-slate-900 dark:text-slate-200 items-center justify-between rounded-md transition-all px-2 py-1 flex hover:bg-slate-900/10 dark:hover:bg-slate-700" target="_blank" href="{resume}">
                            Resume
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="transition-all group-hover:opacity-100 opacity-0 w-5 h-5">
                                <path d="M10.75 2.75a.75.75 0 00-1.5 0v8.614L6.295 8.235a.75.75 0 10-1.09 1.03l4.25 4.5a.75.75 0 001.09 0l4.25-4.5a.75.75 0 00-1.09-1.03l-2.955 3.129V2.75z" />
                                <path d="M3.5 12.75a.75.75 0 00-1.5 0v2.5A2.75 2.75 0 004.75 18h10.5A2.75 2.75 0 0018 15.25v-2.5a.75.75 0 00-1.5 0v2.5c0 .69-.56 1.25-1.25 1.25H4.75c-.69 0-1.25-.56-1.25-1.25v-2.5z" />
                            </svg> 
                        </a>
                        <a class="group md:w-full w-3/5 text-slate-700/80 hover:text-slate-900 dark:text-slate-200 items-center justify-between rounded-md transition-all px-2 py-1 flex hover:bg-slate-900/10 dark:hover:bg-slate-700" href="https://www.linkedin.com/in/tim-phillips-975239b9/">
                            LinkedIn
                            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" class="transition-all group-hover:opacity-100 opacity-0 w-5 h-5">
                                <path fill-rule="evenodd" d="M5.22 14.78a.75.75 0 001.06 0l7.22-7.22v5.69a.75.75 0 001.5 0v-7.5a.75.75 0 00-.75-.75h-7.5a.75.75 0 000 1.5h5.69l-7.22 7.22a.75.75 0 000 1.06z" clip-rule="evenodd" />
                            </svg> 
                        </a>
                    </div>
                </div>
            </div>
            <div class="grid gap-3 md:col-span-3">
                <h3 class="text-4xl font-medium">About</h3>
                <p class="">My passion for design centres around the individual details, interactions and systems that work in unison to create cohesive experiences. I enjoy working on projects from scratch and also jumping into existing problem spaces.</p>
                <p class="">I’m currently working as a product designer for <a class={linkStyles} href="https://www.carsales.com.au/">carsales</a>, within their digital retailing team exploring how to bring offline processes within the car buying journey, online within their platform.</p>
                <p>I’ve previously worked at a start up, <a class={linkStyles} href="https://assembler.app/">Assembler</a>, a compliance focused saas platform, leading their product design and front-end development. Prior to that I worked as product designer within <a class={linkStyles} href="https://www.pwc.com.au/">PwC Australia’s</a> New Ventures unit, a digital business/technology incubator, working within the Automation Engine team.</p>
            </div>
        </div>
    </div>
</div>
