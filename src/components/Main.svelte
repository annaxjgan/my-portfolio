<script>
    import Step from "./Step.svelte"

    let benefits =[
        {name:'Master of IT Student', description:'Currently studying Master of IT, Computing at the University of Melbourne'},
        {name:'Data Product Consultant', description:'I have a year of work experience as a Data Consultant in a Software Engineering team.'},
        {name:'', description:''},
    ]

    let steps=[
        {name: 'Personal Website', icon: 'fa-solid fa-user-tie'},
        {name: 'Friendship matching app', icon: 'fa-solid fa-mobile-screen-button'},
    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="g:grid-cols-2 gap-10 py-8 sm:py-14 flex flex-col ">
        <div class="flex flex-col items-center justify-center text-center gap-6 md:gap-8 lg:gap-10 lg:h-auto min-h-screen">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins" style="color: #92d3f7;">Anna Gan</span> <br/><br/>Aspiring <span class="poppins"  style="color: #92d3f7;">Software Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                I enjoy <span class="poppins" style="color: #92d3f7">creating</span> things with <span class="poppins" style="color: #92d3f7">tech</span>
            </p>
            <a class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" 
                href="https://www.linkedin.com/in/annagan/" 
                target="_blank">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 dduration-200"></div>
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>

        <section id="about" class="grid grid-cols-1 top-20 lg:grid-cols-3 gap-10 py-8 sm:py-14 items-center justify-center gap-24 lg:h-auto min-h-screen">
            <div class="relative shadow-2xl grid place-items-center col-span-1">
                <img src={"images/Profile Picture.png"} alt="Profile Image" class="object-cover z-[2] max-h-[70vh]"/>
            </div>
            <div class="flex flex-col gap-6 md:gap-8 lg:gap-10 col-span-2">
                <div class="text-center">
                    <h5 class="font-semibold text-2xl sm:text-3xl md:text-4xl">
                        <span class="poppins" style="color: #ffffff;">About Me</span> 
                    </h5>
                </div>
                <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
                    {#each benefits as benefit, index}
                        <div class="flex gap-6 sm:gap-8">
                            <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold">
                                0{index+1}
                            </p>
                            <div class="flex flex-col gap-6 sm:gap-8">
                                <h5 class="text-2xl sm:text-3xl md:text-5xl">
                                    {benefit.name}
                                </h5>
                                <p class="text-1xl sm:text-2xl md:text-3xl">{benefit.description}</p>
                            </div>
                        </div>
                    {/each}
                </div>
            </div>
        </section>

    <section id="projects" class="py-20 lg:py-32 gap-24 lg:h-auto min-h-screen">
        <div class="text-center flex flex-col gap-2 h-[150px]">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                Projects I've done.
            </h6>
        </div>
        <div class="flex flex-wrap gap-12">
            <div class="flex-1 min-w-[calc(50%-1.5rem)] h-[200px]">
                <Step step={steps[0]}>
                    <p>This is the website you're viewing right now. <br/>Created with <strong style="color: #92d3f7;">HTML, CSS, JavaScript & Svelte</strong></p>
                </Step>
            </div>
            <div class="flex-1 min-w-[calc(50%-1.5rem)] h-[200px]">
                <Step step={steps[1]}>
                    <p>Friendship app is a mobile app that matches friends of the same interests.<br/>Created with <strong style="color: #92d3f7;">Python, Java, Flask, Figma & AndroidStudio</strong></p>
                </Step>
            </div>

        </div>
    </section>

        
        
    </section>
</main>