<script setup lang="ts">
	definePageMeta({
		// layout: 'default',
		// name: 'slug',
		// alias: 'slug',
	  title: 'Slug',
	   description: 'Slug',
	   // hidden: true,
		navOrder: '3',
		type: 'primary',
    icon: 'i-mdi-home',
    // ogImage: 'images/ogImage.png', // url or local images inside public folder, for eg, ~/public/images/ogImage.png
	})

	 // import { computed } from 'vue'
		// import { useArticles } from '~/composables/articles'

		// const articleId = useRoute().params.id

		// const { data: article } = await useAsyncData('articles', async () => {
		// 	const { getArticle } = useArticles()
		// 	return await getArticle(+articleId)
		// })

	const route = useRoute()
	const capitalize = s => (s && s[0].toUpperCase() + s.slice(1)) || ''
	 useServerSeoMeta({
	   description: () => capitalize(route.params.slug),
	 })
	 useHead({
	   title: () => capitalize(route.params.slug),
	 })
     const slug = route.params.slug
     const title = capitalize(route.params.slug).replaceAll('-', ' ')
</script>

<template layout="default">
	<div><article class="max-w-4xl mx-auto px-4 py-12">
    <div class="mb-8">
        <img src="https://images.unsplash.com/photo-1528712306091-ed0763094c98?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDJ8fHRhbWlsJTIwY29va2luZ3xlbnwwfHx8fDE3MzI3ODU1MzJ8MA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop" alt="Traditional Tamil Cooking" class="w-full h-[400px] object-cover rounded-lg shadow-lg">
    </div>
    
    <div class="space-y-6">
        <div class="flex items-center gap-4 text-primary-600">
            <time datetime="2024-01-15">January 15, 2024</time>
            <span>•</span>
            <span>Tamil Cuisine</span>
        </div>

        <h1 class="font-serif text-4xl md:text-5xl text-primary-800 mb-4">{{ title }}</h1>
        
        <div class="flex items-center gap-4 mb-8">
            <img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixid=M3wyMDkyMnwwfDF8c2VhcmNofDE1fHxmYXRoaW1hJTIwcHJvZmlsZXxlbnwwfHx8fDE3MzI3ODY1NTR8MA&ixlib=rb-4.0.3q=85&fm=jpg&crop=faces&cs=srgb&w=1200&h=800&fit=crop" alt="Fathima Kaja" class="w-12 h-12 rounded-full">
            <div>
                <p class="font-medium text-primary-700">Fathima Kaja</p>
                <p class="text-primary-600">Master Chef & Food Historian</p>
            </div>
        </div>

        <p class="text-lg text-primary-700 mb-8">Discover the rich heritage of Tamil cooking, where ancient spices meet traditional techniques to create dishes that have been cherished for generations.</p>

        <div class="prose max-w-none text-primary-700">
            <p>Tamil cuisine is a celebration of flavors, textures, and aromas that have evolved over thousands of years. The careful balance of spices, the importance of traditional cooking vessels, and the ritualistic approach to meal preparation all contribute to the unique character of our dishes.</p>

            <h2 class="font-serif text-2xl text-primary-800 mt-8 mb-4">The Foundation of Tamil Cooking</h2>
            <p>At the heart of Tamil cooking lies the mastery of spice blending. Each household maintains its own closely guarded recipes, passed down through generations. The use of stone grinders, clay pots, and traditional cooking methods ensures that the authentic flavors are preserved.</p>
        </div>

        <div class="flex flex-wrap gap-2 mt-8">
            <span class="px-3 py-1 bg-secondary-100 text-secondary-700 rounded-full">#TamilCuisine</span>
            <span class="px-3 py-1 bg-secondary-100 text-secondary-700 rounded-full">#TraditionalCooking</span>
            <span class="px-3 py-1 bg-secondary-100 text-secondary-700 rounded-full">#CulinaryHeritage</span>
        </div>
    </div>
</article>
		
	</div>
</template>

<style scoped></style>

