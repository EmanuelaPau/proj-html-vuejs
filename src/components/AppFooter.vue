<template>
    <div class="container-fluid">
        <div class="row my_container">
            <div class="col-6">
                <ul class="d-flex flex-wrap list-unstyled">
                    <a class="text-reset text-decoration-none" href="">
                        <li class="me-4">Term and Conditions</li>
                    </a>
                    <a class="text-reset text-decoration-none" href="">
                        <li class="me-4">Policy</li>
                    </a>
                    <a class="text-reset text-decoration-none" href="">
                        <li class="me-4">About</li>
                    </a>
                </ul>
            </div>
            <div class="col-6 d-flex flex-wrap justify-content-end px-0">
                <span class="me-1">
                    © 2020
                </span>
                <span class="txtColorPrimary me-1">
                    @Themepul
                </span>
                <span>
                    All Rights Reserved.
                </span>
            </div>
        </div>
    </div>
</template>

<script>
//  import HelloWorld from './HelloWorld.vue'

export default {
    name: 'AppFooter',
    components: {
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
@use '../styles/partials/_variables.scss';
@use '../styles/partials/_mixins.scss';
</style> 
