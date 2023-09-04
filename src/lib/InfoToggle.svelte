<script>
    function toggleInfo() {
        let btn = document.getElementById('info-btn')
        let text = btn.innerHTML;
        btn.innerHTML = text == 'Less info' ? 'More info' : 'Less info';

        let info = document.getElementById('info-col')
        info.classList.toggle('hidden');
    }
</script>

<button on:click={toggleInfo} id="info-btn" class="md:hidden inline-flex transition-all px-4 py-2 font-medium text-sm text-slate-100 bg-slate-800 border border-slate-800 rounded-lg drop-shadow-sm hover:bg-slate-900 hover:border-slate-950 hover:drop-shadow-lg hover:text-white">
    More info  
</button>