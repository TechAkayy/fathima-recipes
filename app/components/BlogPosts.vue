<script setup lang="ts">
	// const props = defineProps({
	// 	name: {
	// 		type: String,
	// 		default: 'BlogPosts',
	// 	},
	// })

	// const emit = defineEmits(['addToCart'])

	// // Use the addToCart function like this:
	// // Eg-1: addToCart('pizza', 10)
	// // Eg-2: (event) => addToCart('pizza', 10, event)
	// const addToCart = (item, quantity /*, event*/) => {
	// 	emit('addToCart', { item, quantity })
	// }
</script>

<template><section class="py-16 px-4 sm:px-6 lg:px-8 bg-stone-100">
    <div class="max-w-7xl mx-auto">
        <h2 class="text-3xl md:text-4xl font-serif text-primary-800 text-center mb-12">Latest Culinary Stories</h2>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            <article class="bg-white rounded-lg overflow-hidden shadow-lg">
                <img src="https://images.unsplash.com/photo-1481016863889-534cbad65379?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE1fHx0cmFkaXRpb25hbCUyMGNvb2tpbmd8ZW58MHx8fHwxNzMyNzA3MDgzfDA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop" alt="Traditional Tamil Cooking Methods" class="w-full h-64 object-cover"/>
                <div class="p-6">
                    <div class="text-secondary-600 text-sm mb-2">March 15, 2024</div>
                    <h3 class="font-serif text-xl text-primary-900 mb-3">The Art of Traditional Tamil Spice Blending</h3>
                    <p class="text-gray-600 mb-4">Discover the secrets behind creating authentic Tamil spice blends that have been passed down through generations...</p>
                    <NuxtLink class="text-primary-600 hover:text-primary-700 font-sans" to="/tamil-spice-blending">Read More →</NuxtLink>
                </div>
            </article>
            <article class="bg-white rounded-lg overflow-hidden shadow-lg">
                <img src="https://images.unsplash.com/photo-1697070318586-66eb79cd71e4?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDl8fGZlc3RpdmFsJTIwZm9vZHxlbnwwfHx8fDE3MzI3ODU1OTl8MA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop" alt="Tamil Festival Foods" class="w-full h-64 object-cover"/>
                <div class="p-6">
                    <div class="text-secondary-600 text-sm mb-2">March 10, 2024</div>
                    <h3 class="font-serif text-xl text-primary-900 mb-3">Festival Foods: Celebrating Tamil Heritage</h3>
                    <p class="text-gray-600 mb-4">Explore the rich tradition of festival cooking in Tamil culture and learn about special dishes prepared...</p>
                    <NuxtLink class="text-primary-600 hover:text-primary-700 font-sans" to="/festival-foods">Read More →</NuxtLink>
                </div>
            </article>
            <article class="bg-white rounded-lg overflow-hidden shadow-lg">
                <img src="https://images.unsplash.com/photo-1507089947368-19c1da9775ae?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDJ8fGtpdGNoZW4lMjB0aXBzfGVufDB8fHx8MTczMjc4NTYwMHww&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop" alt="Kitchen Tips and Techniques" class="w-full h-64 object-cover"/>
                <div class="p-6">
                    <div class="text-secondary-600 text-sm mb-2">March 5, 2024</div>
                    <h3 class="font-serif text-xl text-primary-900 mb-3">Essential Tamil Kitchen Tips and Techniques</h3>
                    <p class="text-gray-600 mb-4">Master the fundamental techniques of Tamil cooking with these time-tested kitchen tips and methods...</p>
                    <NuxtLink class="text-primary-600 hover:text-primary-700 font-sans" to="/kitchen-tips">Read More →</NuxtLink>
                </div>
            </article>
        </div>
    </div>
</section></template>

<style scoped></style>

