<script>
export default {
    props: {
        description: {
            type: String,
            default: ''
        }
    }
}
</script>

<template>
    <section class="flex items-center justify-center">
        <div class="my-40">
            <svg class="h-64 w-64" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 36 36">
                <circle fill="#F3F3F3" cx="18" cy="18" r="14.5" />
                <path fill="#FFFFFF" d="M17.343 20.748l8.777 5.381-5.379-8.778z" />
                <path fill="#FFFFFF" d="M18.657 15.267L9.879 9.886l5.38 8.779z" />
                <circle fill="#FFFFFF" cx="18" cy="18.008" r="3.055" />
                <circle fill="#F3F3F3" cx="18" cy="18.008" r="1.648" /></svg>

            <slot>
                <p class="text-center text-gray-500">{{ description }}</p>
            </slot>
        </div>
    </section>
</template>
