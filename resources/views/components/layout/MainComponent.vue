<template>
    <div class="container">
        <main class="d-flex flex-wrap pt-3">
          <CardComponent
            v-for="(item, index) in items"
            :key="index"
            :data="item"
            class="card-item m-1"
          />
        </main>
    </div>
</template>

<script>
import CardComponent from '../utils/CardComponent.vue';

export default {
    name: "LayoutComponent",
    components: {
        CardComponent
    },
    data() {
        return {
            items: [
                { title: 'Tryout 1', creator: 'Yuda 1' },
                { title: 'Tryout 2', creator: 'Yuda 2' },
                { title: 'Tryout 3', creator: 'Yuda 3' },
                { title: 'Tryout 4', creator: 'Yuda 4' },
                { title: 'Tryout 5', creator: 'Yuda 5' },
                { title: 'Tryout 6', creator: 'Yuda 6' },
                { title: 'Tryout 7', creator: 'Yuda 7' },
                { title: 'Tryout 8', creator: 'Yuda 8' },
            ],
        };
    }
}
</script>

<style scoped></style>
