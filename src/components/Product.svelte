<script>
    import ProductCard from "./ProductCard.svelte"
    import SectionWrapper from "./SectionWrapper.svelte"

    let productFeatures = [
        {
            featureList: [
                "Daily streak counter",
                "Weights and reps tracker",
                "Community challenges",
                "Every workout is new and exciting",
            ],
            description: "Hakuna Matata ensures all users have the information they need to train safely and train effectively.",
            imgUrl:"assets/selection.png",
        },
        {
            featureList: [
                "Select your preferences",
                "Personalize your workouts",
                "Customize your training",
                "Guarantees progress on all core exercises",
            ],
            description:"Build you streaks and see your progress with our amazing tracking and analytics features.",
            imgUrl:"assets/goal.png"
        },
        {
            featureList: [
                "Eliminating guesswork",
                "Save time",
                "Achieve the performance you seek",
                "Builds functional strength",
            ],
            description:"Enter as much information about yourself as you desire to ensure all workouts are personalized to your every need.",
            imgUrl:"assets/training.png",
        },
    ];
</script>
<SectionWrapper id="product">
    <div class="flex flex-col justify-center items-center gap-10 sm:gap-14 md:gap-24 flex-1 pb-10 md:pb-14">
        <div class="flex flex-col gap-2">
            <p class="text-base sm:text-lg md:text-xl text-center opacity-60">
                Start your <span class="text-indigo-400">Gym Streak</span> today
            </p>
            <h3 class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center">
                Features For <span class="text-indigo-400">Everyone</span>
            </h3>
        </div>
        {#each productFeatures as productFeature, index}
            <ProductCard {productFeature} {index}>
                {#if index===0}
                Experience a beginner exercise <span class="text-indigo-400 font-medium">Master</span> class
                {:else if index===1}
                Lay the foundations for <span class="text-indigo-400 font-medium">Routine</span> and consistency
                {:else}
                Workouts specefic to your <span class="text-indigo-400 font-medium">Environment</span> and <span class="text-indigo-400 font-medium">Expertise</span>
                {/if}
            </ProductCard>
        {/each}
    </div>
</SectionWrapper>