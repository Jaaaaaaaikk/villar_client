<template>
    <div class="text-box">
        <label :for="id" class="label">{{ label }}</label>
        <input :id="id" :type="type" :value="value" :placeholder="placeholder"
            @input="$emit('input', $event.target.value)" class="input" required/>
    </div>
</template>

<script>
export default {
    props: {
        id: {
            type: String,
            required: true,
        },
        label: {
            type: String,
            required: true,
        },
        type: {
            type: String,
            default: 'text',
        },
        value: {
            type: String,
            default: '',
        },
        placeholder: {
            type: String,
            default: '',
        },
    },
};
</script>

<style scoped>
.text-box {
    margin-bottom: 1rem;
}

.label {
    display: block;
    font-weight: bold;
    margin-bottom: 0.5rem;
}

.input {
    width: 100%;
    padding: 0.5rem;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 1rem;
}
</style>