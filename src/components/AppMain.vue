<template>
    <main>
        <MainMail />
    </main>
</template>

<script>
//  import HelloWorld from './HelloWorld.vue'
import MainMail from './Main/MainMail.vue'
export default {
    name: 'AppMain',
    components: {
        MainMail
    },
    data() {
        return {

            // links: [
            //	'gino',
            //	'ciao',
            //	]


        }
    },
    methods() {
    },
}		
</script>
<style scoped lang="scss">
@use '../styles/general.scss';
@use '../styles/partials/_mixins.scss';
@use '../styles/partials/variables.scss';
</style> 
