<template>
    <div id="services">
        <div class="service" v-for="service in mockData">
            <ServiceTile :header="service.header" :description="service.description" :imagePath="service.imgUrl"
                :price="service.price"></ServiceTile>
        </div>
    </div>
</template>

<script setup>
import ServiceTile from '../components/ServiceTile.vue';
const mockData = [
    {
        header: 'manikura',
        description: 'Whereas a common understanding of these rights and freedoms is ',
        imgUrl: 'https://images.unsplash.com/photo-1599206676335-193c82b13c9e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=707&q=80',
        price: 0,
    },
    {
        header: 'trhani oboci',
        description: 'Whereas a common understanding of these rights and freedoms is ',
        imgUrl: 'https://images.unsplash.com/photo-1519415387722-a1c3bbef716c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80',
        price: 0,
    },
    {
        header: 'make-up',
        description: 'home or correspondence, nor to attacks upon his honour and reputation. Everyone has the right to the protection of the law against such interference or attacks. ',
        imgUrl: 'https://images.unsplash.com/photo-1596205521983-9c372fb3d4f1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=764&q=80',
        price: 0,
    },

    {
        header: 'make-up',
        description: 'home or correspondence, nor to attacks upon his honour and reputation. Everyone has the right to the protection of the law against such interference or attacks. ',
        imgUrl: 'https://images.unsplash.com/photo-1596205521983-9c372fb3d4f1?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=764&q=80',
        price: 0,
    },
    {
        header: 'trhani oboci',
        description: 'Whereas a common understanding of these rights and freedoms is ',
        imgUrl: 'https://images.unsplash.com/photo-1519415387722-a1c3bbef716c?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80',
        price: 0,
    },
    {
        header: 'manikura',
        description: 'description',
        imgUrl: 'https://images.unsplash.com/photo-1599206676335-193c82b13c9e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=707&q=80',
        price: 0,
    },

]
</script>

<style scoped>
#services {
    display: grid;
    width: 100%;
    grid-template-columns: 1fr 1fr 1fr;
    grid-auto-rows: 1fr;
}

.service {
    width: 80%;
    margin: auto;
    margin-top: 1rem;
    text-align: center;
    padding: 1rem;
}

.service:nth-child(3n - 1) {
    margin-top: 5rem;
}


@media (min-width: 1024px) {}
</style>
  