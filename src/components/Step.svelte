<script>
    export let step;
</script>

<a href={step.href} target="_blank">

</a>
<a href={"step.href"} target="_blank" class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid text-center group cursor-pointer hover:border-blue-400 duration-200 h-[280px]" style="color: #ffffff;">
    <div class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200">
        <i class={step.icon}/>
    </div>
    <h3 class="font-medium text-xl sm:text-3xl" style="color: #ffffff;">{step.name}</h3>
    <slot/>
    <div class="flex-1 flex justify-between gap-4 items-center">
        <div class="ml-auto cursor-pointer hover:text-slate-950 duration-200 relative after:absolute after:bg-white after:top-0 after:h-0 after:right-full after:w-full after:h-full after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden">
            <a href="https://github.com/annaxjgan/my-website1" target="_blank">
                <p class="relative z-4">Go to &rarr;</p>
            </a>
            
        </div>
    </div>
</a>