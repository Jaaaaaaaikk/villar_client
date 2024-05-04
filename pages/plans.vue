<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold mb-8">Pricing Plans</h1>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
            <div v-for="(plan, index) in plans" :key="index" class="bg-white shadow-md rounded-lg p-6">
                <h2 class="text-xl font-semibold mb-4">{{ plan.name }}</h2>
                <p class="text-gray-700 mb-4">{{ plan.description }}</p>
                <div class="text-3xl font-bold mb-4">${{ plan.price }}/month</div>
                <button class="bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-2 px-4 rounded">
                    Choose Plan
                </button>
            </div>
        </div>
        <NuxtLink to="/dashboard"
            class="mt-8 inline-block bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-2 px-4 rounded">
            Back to Homepage
        </NuxtLink>
    </div>
</template>

<script>
export default {
    data() {
        return {
            plans: [
                {
                    name: 'Basic',
                    description: 'Suitable for small businesses and startups.',
                    price: 9.99,
                    features: [
                        '10 GB storage',
                        '1 user account',
                        'Basic support',
                    ],
                },
                {
                    name: 'Pro',
                    description: 'Ideal for growing businesses with increased needs.',
                    price: 19.99,
                    features: [
                        '50 GB storage',
                        '5 user accounts',
                        'Priority support',
                        'Advanced analytics',
                    ],
                },
                {
                    name: 'Enterprise',
                    description: 'Tailored for large organizations with custom requirements.',
                    price: 49.99,
                    features: [
                        'Unlimited storage',
                        'Unlimited user accounts',
                        'Dedicated support',
                        'Custom integrations',
                        'SSO (Single Sign-On)',
                    ],
                },
            ],
        };
    },
};
</script>

<style scoped></style>