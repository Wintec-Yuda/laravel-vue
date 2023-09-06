<template>
    <div>
        <HeaderComponent />
        <MainComponent />
        <FooterComponent />
    </div>
</template>

<script>
import HeaderComponent from './layout/HeaderComponent.vue';
import MainComponent from './layout/MainComponent.vue';
import FooterComponent from './layout/FooterComponent.vue';

export default {
    components: {
        HeaderComponent,
        MainComponent,
        FooterComponent
    }
}
</script>
