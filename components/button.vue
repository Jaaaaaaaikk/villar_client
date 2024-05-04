<template>
    <button class="modern-button" :class="{ 'is-disabled': disabled }" @click="onClick" :disabled="disabled">
        <slot></slot>
    </button>
</template>

<script>
export default {
    props: {
        disabled: {
            type: Boolean,
            default: false,
        },
    },
    methods: {
        onClick(event) {
            if (!this.disabled) {
                this.$emit('click', event);
            }
        },
    },
};
</script>

<style scoped>
.modern-button {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    font-size: 1rem;
    font-weight: bold;
    text-align: center;
    text-decoration: none;
    color: #fff;
    background-color: #0a4e9b;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.modern-button:hover {
    background-color: #5a3ace;
}

.modern-button:focus {
    outline: none;
    box-shadow: 0 0 0 3px rgba(74, 144, 226, 0.3);
}

.modern-button.is-disabled {
    background-color: #ccc;
    cursor: not-allowed;
}
</style>