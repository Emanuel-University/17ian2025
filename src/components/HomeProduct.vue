<script setup>
 const props = defineProps(["image", "title", "rates", "reviews", "price"])
</script>

<template>
    <div class="w-full flex flex-col bg-blue-200 p-2 rounded-md drop-shadow-md">
        <img :src="props.image.link" :alt="props.image.alt">
        <div> {{ props.title }} </div>
        <div> {{ props.rates }} <span> {{ props.reviews }}</span> </div>
        <div> {{ props.price }} </div>
        <button>Add To Cart</button>
    </div>
</template>