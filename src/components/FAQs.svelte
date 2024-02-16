<script>
  import SectionWrapper from "./SectionWrapper.svelte";
  let faq = [
  {
    question: "What is the purpose of this fitness program website?",
    answer: "Our fitness program website is designed to provide you with comprehensive workout plans, nutrition guidance, and support to help you achieve your fitness goals."
  },
  {
    question: "How do I get started with the fitness program?",
    answer: "To get started, simply sign up on our website, create an account, and choose a suitable fitness program based on your goals. Follow the instructions to begin your fitness journey."
  },
  {
    question: "Are the workout programs suitable for beginners?",
    answer: "Yes, we offer a variety of programs tailored for all fitness levels, including beginners. You can select a program that matches your current fitness level and gradually progress as you get stronger."
  },
  {
    question: "Can I customize my workout plan?",
    answer: "Absolutely! Our platform allows you to customize your workout plan based on your preferences, fitness level, and any specific requirements you may have. Personalization is key to your success."
  },
  {
    question: "What type of exercises are included in the programs?",
    answer: "Our programs include a mix of cardiovascular exercises, strength training, flexibility routines, and more. The variety ensures a well-rounded approach to fitness, targeting different aspects of your health."
  },
  {
    question: "Is nutritional guidance provided?",
    answer: "Yes, we offer nutritional guidance to complement your fitness journey. You'll find information on healthy eating habits, meal plans, and dietary tips to enhance your overall well-being."
  },
  {
    question: "How can I track my progress?",
    answer: "We provide tools and features to track your fitness progress. You can log your workouts, monitor changes in your measurements, and even set and achieve milestones. This helps you stay motivated and focused on your goals."
  },
  {
    question: "Is there a community or support system on the website?",
    answer: "Certainly! We have a supportive community where you can connect with fellow members, share your experiences, and seek advice. Our forums and chat features are there to help you stay motivated and accountable."
  },
  {
    question: "Can I access the fitness programs on mobile devices?",
    answer: "Yes, our website is mobile-friendly, allowing you to access your fitness programs and resources on the go. You can use your smartphone or tablet to stay connected and committed to your fitness routine."
  },
  {
    question: "How can I contact customer support if I have any issues?",
    answer: "If you have any questions or encounter issues, you can reach out to our customer support team through the contact form on our website. We are here to assist you and ensure you have a positive experience with our fitness program."
  }
]


</script>
<SectionWrapper id="faq">
    <div class="flex flex-col gap-10 sm:gap-14 md:gap-24 py-20 flex-1 items-center justify-center">
        <div class="flex flex-col gap-2">
            <p class="opacity-80 text-base sm:text-lg md:text-xl text-center">
                For All Your Questions, Hakunas and Matatas
            </p>
            <h3 class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center">
                Frequently <span class="text-indigo-400">Asked</span> Questions
            </h3>
        </div>
        <div class="flex flex-col gap-8 sm:gap-10 md:gap-14 w-full">
            {#each faq as faqq}
                <div class="flex flex-col gap-2 text-left max-w-[800px] w-full mx-auto relative p-4 px-6">
                    <div class="absolute top-0 left-0 w-1/3 h-[2px] bg-indigo-400 -translate-x-4"></div>
                    <div class="absolute top-0 left-0 w-[2px] h-2/3 bg-indigo-400 -translate-y-4"></div>
                    <h4 class="text-lg sm:text-xl md:text-2xl pt-2">{faqq.question}</h4>
                    <p class="pl-2">{faqq.answer}</p>
                </div>
            {/each}
        </div>
    </div>
</SectionWrapper>