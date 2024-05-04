<template>
    <div class="flex flex-col min-h-screen bg-blue-400">
        <div class="flex-grow flex items-center justify-center">
            <div class="text-center">
                <h1 class="text-4xl font-bold mb-6">Welcome to Jaikhene Website</h1>
                <button @click="navigateToHome"
                    class="bg-blue-900 hover:bg-blue-600 text-white font-semibold py-2 px-4 rounded">
                    Get Started
                </button>
            </div>
        </div>

        <footer class="bg-gray-800 text-white py-4">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="text-center">
                    <p class="text-gray-400">&copy; 2024 Jaikhene Website. All rights reserved.</p>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    methods: {
        navigateToHome() {
            this.$router.push({ path: '/dashboard'});
        },
    },
};
</script>

<style scoped>
template {
    background-color: aqua;
    min-height: 100vh;
}
</style>