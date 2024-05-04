<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold mb-8">Frequently Asked Questions</h1>
        <div class="space-y-6">
            <div v-for="(faq, index) in faqs" :key="index" class="bg-white shadow-md rounded-lg p-6">
                <h2 class="text-xl font-semibold mb-2">{{ faq.question }}</h2>
                <p class="text-gray-700">{{ faq.answer }}</p>
            </div>
        </div>
        <NuxtLink to="/dashboard"
            class="mt-8 inline-block bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-2 px-4 rounded mb-4">
            Back to Homepage
        </NuxtLink>
    </div>
</template>

<script>
export default {
    data() {
        return {
            faqs: [
                {
                    question: 'What is Nuxt.js?',
                    answer: 'Nuxt.js is a progressive framework for building Vue.js applications...',
                },
                {
                    question: 'What are the benefits of using Nuxt.js?',
                    answer: 'Nuxt.js offers several benefits, including automatic code splitting, server-side rendering, powerful routing, static site generation, and a modular architecture. It helps improve performance, SEO, and development productivity.',
                },
                {
                    question: 'Is Nuxt.js suitable for building large-scale applications?',
                    answer: 'Yes, Nuxt.js is well-suited for building large-scale applications. Its modular architecture, code splitting, and server-side rendering capabilities make it scalable and maintainable. It also provides a powerful plugin system and integrates well with various libraries and frameworks.',
                },
                {
                    question: 'Can I use Nuxt.js with other UI libraries or frameworks?',
                    answer: 'Absolutely! Nuxt.js is compatible with various UI libraries and frameworks. You can easily integrate popular libraries like Vuetify, Bootstrap Vue, or Tailwind CSS into your Nuxt.js projects. Nuxt.js provides a flexible and extensible architecture that allows seamless integration with different tools and libraries.',
                },
                {
                    question: 'How does Nuxt.js handle routing?',
                    answer: 'Nuxt.js provides a powerful and intuitive routing system out of the box. It automatically generates Vue Router configuration based on your project\'s directory structure. You can define routes by creating .vue files in the pages directory, and Nuxt.js will automatically handle the routing for you.',
                },
                {
                    question: 'Can I use server-side rendering (SSR) with Nuxt.js?',
                    answer: 'Yes, Nuxt.js fully supports server-side rendering. By default, Nuxt.js applications are server-rendered, which means the initial page load is rendered on the server and sent to the client. This improves the application\'s performance, SEO, and initial load time. You can also configure Nuxt.js for client-side rendering if needed.',
                },
                {
                    question: 'How can I deploy a Nuxt.js application?',
                    answer: 'Nuxt.js provides various deployment options. You can deploy your Nuxt.js application to static hosting platforms like Netlify, Vercel, or GitHub Pages by generating a static version of your application using the nuxt generate command. You can also deploy to server environments like Node.js servers or serverless platforms like AWS Lambda.',
                },
                {
                    question: 'Does Nuxt.js support static site generation?',
                    answer: 'Yes, Nuxt.js has excellent support for static site generation. With the nuxt generate command, you can generate a fully static version of your Nuxt.js application. This allows you to host your application on static hosting platforms and enjoy the benefits of fast page loads and easy deployment.',
                },
                {
                    question: 'Can I use Nuxt.js with a headless CMS?',
                    answer: 'Absolutely! Nuxt.js integrates well with headless CMS solutions. You can fetch content from a headless CMS using Nuxt.js\'s powerful data fetching methods, such as asyncData or fetch. Nuxt.js provides a seamless way to integrate your application with popular headless CMS platforms like Contentful, Strapi, or Prismic.',
                },
                {
                    question: 'Is Nuxt.js open-source and free to use?',
                    answer: 'Yes, Nuxt.js is an open-source framework released under the MIT license. It is freely available for developers to use, modify, and distribute. You can find the source code and contribute to the Nuxt.js project on GitHub.',
                },
            ],
        };
    },
};
</script>

<style scoped></style>