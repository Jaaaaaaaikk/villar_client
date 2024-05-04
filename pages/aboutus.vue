<template>
    <div class="about-us">
        <h1 class="text-3xl font-bold mb-4">About Us</h1>
        <p class="mb-6">
            Welcome to our website! We are a passionate team of developers and designers dedicated to creating
            innovative and high-quality web applications using Nuxt.js.
        </p>
        <p class="mb-6">
            At our company, we believe in the power of Nuxt.js to build modern, performant, and scalable applications.
            With its intuitive structure, server-side rendering capabilities, and excellent developer experience,
            Nuxt.js allows us to deliver exceptional results to our clients.
        </p>
        <h2 class="text-2xl font-bold mb-4">Our Mission</h2>
        <p class="mb-6">
            Our mission is to empower businesses and individuals by providing cutting-edge web solutions. We strive to
            understand our clients' unique requirements and goals, and we work closely with them to develop tailored
            applications that exceed their expectations.
        </p>
        <h2 class="text-2xl font-bold mb-4">Our Expertise</h2>
        <p class="mb-6">
            Our team consists of skilled professionals with extensive experience in Nuxt.js development. We stay
            up-to-date with the latest trends and best practices in the Vue.js ecosystem, ensuring that our projects are
            built using the most efficient and reliable techniques.
        </p>
        <p class="mb-6">
            Whether you need a simple brochure website, a complex web application, or anything in between, we have the
            expertise to deliver outstanding results. We are committed to writing clean, maintainable, and optimized
            code that adheres to industry standards.
        </p>
        <h2 class="text-2xl font-bold mb-4">Our Process</h2>
        <p class="mb-6">
            We follow a collaborative and iterative process to ensure the success of every project. From initial
            consultation and planning to design, development, and deployment, we work closely with our clients at every
            stage. We value open communication, transparency, and a client-centric approach.
        </p>
        <p class="mb-6">
            Our goal is to not only deliver a high-quality product but also to provide an exceptional experience for our
            clients. We strive to build long-term partnerships based on trust, reliability, and mutual success.
        </p>
        <h2 class="text-2xl font-bold mb-4">Get in Touch</h2>
        <p>
            If you have a project in mind or would like to learn more about our services, we'd love to hear from you.
            Feel free to reach out to us using the contact information below, and one of our friendly team members will
            get back to you shortly.
        </p>
    </div>
    <NuxtLink to="/dashboard"
        class="mt-8 inline-block bg-indigo-600 hover:bg-indigo-700 text-white font-semibold py-2 px-4 rounded mb-4 ml-4">
        Back to Homepage
    </NuxtLink>
</template>

<script>
</script>

<style scoped>
.about-us {
    max-width: 800px;
    margin: 0 auto;
    padding: 2rem;
}
</style>