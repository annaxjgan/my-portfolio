<script>
    export let y;
    let tabs = [
        {name: 'About Me', link: '#about'},
        {name: 'Projects', link: '#projects'},
        {name: 'Contact', link: '#contacts'},
    ];
</script>

<header class={'sticky z-[10] w-full top-0 duration-200 flex items-center justify-between border border-solid ' + (
    y>0 ? 'py-4 bg-slate-950 border-blue-950 ' : ' py-6 bg-transparent border-transparent'
)}>
    <h1 class="font-medium">
        <b class="font-bold poppins">Hello. </b> 
    </h1>
    <div class="sm:flex items-center gap-4 hidden ">
        {#each tabs as tab, index}
            <a href={tab.link} class="duration-200 hover:text-[var(--custom-hover-color)]">
                <p>{tab.name}</p>
            </a>
        {/each}
    </div>
    <a 
    href="https://www.linkedin.com/in/annagan/"
    target="_blank"
    class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950">
        <div class="absolute top-0 right-full w-full h-full bg-blue-400 opacity-20 group-hover:translate-x-full z-0 dduration-200"></div>
        <h4 class="relative z-9">Get in touch</h4>
    </a>
</header>
