<script>
    import SectionWrapper from "./SectionWrapper.svelte"
    import Header from "./Header.svelte"
    import CTA from "./CTAs.svelte"
  import Stars from "./stars.svelte";
</script>
<SectionWrapper>
    <Header/>
    <div class="flex flex-col gap-10 flex-1 items-center justify-center pb-10 md:pb-14">
        <h2 class="text-5xl sm:text-6xl md:text-7xl lf:text-8xl max-w-[1400px] mx-auto w-full text-center font-semibold">
            <span class="text-indigo-400">Gym</span> Training <span class="text-slate-600 line-through">Is Hard</span><br/>
            Just Got <span class="text-indigo-400">Easier</span>
        </h2>
        <p class="text-xl sm:text-2xl md:text-3xl text-center max-w-[1000px] mx-auto w-full">Less thinking and more doing. We're the trainer in your pocket full of <span class="text-indigo-400">personalized workouts, exercises, personalized explainations, analytics</span> and much much more..</p>
        <CTA/>
        <Stars/>
    </div>
</SectionWrapper>