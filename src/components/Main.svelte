<script>
    import Step from "./Step.svelte"

    let steps=[
        {name: 'Personal Website', icon: 'fa-solid fa-user-tie'},
        {name: 'Friend-matching app', icon: 'fa-solid fa-mobile-screen-button'},
    ]
</script>

<main class="flex flex-col flex-1 p-4">
    <section id="introPage" class="g:grid-cols-2 gap-10 py-8 sm:py-14 flex flex-col fade-in">
        <div class="flex flex-col items-center justify-center text-center gap-6 md:gap-8 lg:gap-10 min-h-screen">
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi ! I'm <span class="poppins" style="color: #92d3f7;">Anna.</span> 
            </h2>
            <br/><br/>
            <h2 class="font-semibold text-2xl sm:text-3xl md:text-4xl">
                I enjoy creating <span class="poppins"  style="color: #92d3f7;"> fun </span> stuff with <span class="poppins"  style="color: #92d3f7;"> tech </span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                Passionate about <span class="poppins" style="color: #92d3f7">Software Development</span> and <span class="poppins" style="color: #92d3f7">Cloud Solutions</span>
            </p>
        </div>

        <section id="about" class="grid grid-cols-1 top-20 lg:grid-cols-3 gap-10 py-8 sm:py-14 items-center justify-center gap-24 lg:h-auto min-h-screen fade-in">
            <div class="relative shadow-2xl grid place-items-center col-span-1">
                <img src="images/Profile Picture.png" alt="Profile Image" class="object-cover z-[2] max-h-[70vh]" />
            </div>
            <div class="flex flex-col gap-6 md:gap-8 lg:gap-10 col-span-2">
                <div>
                    <p class="poppins">
                        As an enthusiastic learner, I am always actively learning new skills. 
                        I am proficient in a variety of programming languages including <b>Java, Python, C# and JavaScript.</b>
                        <br>
                        <br>
                        <h7 class="font-semibold">
                            <span style="color: #92d3f7;" class="text-sm sm:text-lg md:text-xl">A bit of background...</span>
                        </h7>
                        <br><br>
                        I studied Chemistry with Molecular Physics at Imperial College London.
                        Realising that scientific research was not the right fit for me, I then joined Kubrick Group as a data consultant upon graduating.
                        <br> 
                        <br>
                        During my work as a consultant, I was placed as a technical business analyst at AstraZeneca within a software engineering team. 
                        This experience became the catalyst for my interest in software development and the tech field.
                        <br>
                        <br>
                        I am currently a First-Year Master's student in IT, Computing at the Univeristy of Melbourne. I am always on the go — 
                        constantly seeking opportunities to work on interesting projects to refine my skills.
                        <br>
                        <br>
                        In my free time, I enjoy playing tennis (albeit not being good at it), drawing, exploring the city, and indulging in occassional daydreaming.
                    </p>
                </div>
            </div>
        </section>

    <section id="projects" class="py-20 lg:py-32 gap-24 lg:h-auto min-h-screen">
        <div class="text-center flex flex-col gap-2 h-[150px]">
            <h6 class="font-semibold text-2xl sm:text-3xl md:text-4xl">
                My <span style="color: #92d3f7;">Projects</span>
            </h6>
        </div>
        <div class="flex flex-wrap gap-12">
            <div class="flex-1 min-w-[calc(50%-1.5rem)] h-[200px]">
                <Step step={steps[0]}>
                    <p>My personal website. <br/>Built using: <strong style="color: #92d3f7;">HTML, CSS, JavaScript & Svelte</strong></p>
                </Step>
            </div>
            <div class="flex-1 min-w-[calc(50%-1.5rem)] h-[200px]">
                <Step step={steps[1]}>
                    <p>A mobile app that matches friends of the same interests.<br/>Built using: <strong style="color: #92d3f7;">Python, Java, Flask, Figma & AndroidStudio</strong></p>
                </Step>
            </div>

        </div>
    </section>

        
        
    </section>
</main>
