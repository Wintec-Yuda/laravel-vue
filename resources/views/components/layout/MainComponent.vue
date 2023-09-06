<template>
    <div>
        <main class="d-flex justify-content-evenly">
            <CardComponent v:for="(item, index) in items" :key="index" :data="item" />
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
            ],
        };
    }
}
</script>

<style scoped></style>