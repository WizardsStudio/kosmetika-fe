<template>
    <div class="image-container">
        <img class="service-image" :src="imagePath">
    </div>
    <h2>{{ header }}</h2>
    <div class="description-container">{{ description }}</div>
</template>
  
<script>
export default {
    props: ['header', 'description', 'imagePath', 'price'],
    setup(props) {
        return {}
    }
}
</script>
<style >
.service-tile {
    width: 60%;

}

h2 {
    color: var(--normal-green);
    font-size: 2rem;
}

.image-container {
    width: 100%;
    aspect-ratio: 1/1;
}

.service-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 50%;
    border: 0.5rem solid var(--normal-green);
}

.description-container {}

@media (min-width: 1024px) {}
</style>
  