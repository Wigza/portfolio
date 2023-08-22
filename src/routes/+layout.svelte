<script>
    import "../app.css";
    import "../global.css";
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Work+Sans:ital,wght@0,300;0,400;0,500;1,300;1,400;1,500&display=swap');
</style>

<nav class="w-full flex items-center justify-between md:mt-6 md:px-6 fixed top-0">
    <div class="flex justify-between md:justify-normal rounded-xl bg-white/75 backdrop-blur-lg border-slate-200 border p-1 shadow shadow-slate-100">
        <a class="font-medium text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900" 
            href="/">
            Tim Phillips, Designer
        </a>
        <a class="text-slate-700 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900" 
            href="/about">
            About
        </a>
    </div>
    <div class="hidden md:flex p-1">
        <a class="text-slate-600 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900" href="#">Resume</a>
        <a class="text-slate-600 px-3 py-0.5 rounded-lg hover:bg-slate-50 hover:text-slate-900 flex items-center" href="www.linkedin.com">
            LinkedIn
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="ml-1 w-5 h-5">
                <path stroke-linecap="round" stroke-linejoin="round" d="M4.5 19.5l15-15m0 0H8.25m11.25 0v11.25" />
            </svg>              
        </a>
    </div>
</nav>


<slot />
