<template>
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold mb-8">Contact Us</h1>
        <form @submit.prevent="submitForm">
            <TextBox id="name" label="Name" v-model="form.name" />
            <TextBox id="email" label="Email" type="email" v-model="form.email" />
            <TextBox id="message" label="Message" v-model="form.message" />
            <button>Send Message</button>
        </form>
        <NuxtLink to="/dashboard"
            class="mt-8 inline-block bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-2 px-4 rounded">
            Back to Homepage
        </NuxtLink>
    </div>
</template>

<script>
import TextBox from '~/components/TextBox.vue';
import button from '~/components/button.vue';

export default {
    components: {
        TextBox,
        button,
    },
    data() {
        return {
            form: {
                name: '',
                email: '',
                message: '',
            },
        };
    },
    methods: {
        submitForm() {
            console.log(this.form);
        },
        handleClick() {
            console.log('Button clicked!');
        },
    },
};
</script>

<style scoped></style>