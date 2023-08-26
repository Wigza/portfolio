<script>
    function toggle() {
        let btn = document.getElementById("menu-btn");
        let menu = document.getElementById("responsive-menu");
        let htmlBody = document.querySelector("html");

        btn.classList.toggle("active");
        menu.classList.toggle("active");
        htmlBody.classList.toggle("overflow-hidden")        
	}
</script>

<style>
    /* active */
    #menu-btn.active svg path.open, #menu-btn svg path.close  {
        visibility: hidden;
    }
    /* inactive */
    #menu-btn.active svg path.close  {
        visibility: visible;
    }
</style>

<button on:click={toggle} id="menu-btn" class="md:hidden text-slate-700 dark:text-slate-300 px-3 py-0.5">
    <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="transition-all w-6 h-6">
        <path stroke-linecap="round" stroke-linejoin="round" d="M3.75 9h16.5m-16.5 6.75h16.5" class="open" />
        <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" class="close" />
      </svg>    
</button>