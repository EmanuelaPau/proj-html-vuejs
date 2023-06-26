<template>
    <div class="">
        <!-- Header top -->
        <div class="line">
            <div class="container-fluid">
                <div class="row py-3 my_container m-auto">
                    <!-- Mail -->
                    <div class="header-mail col-3">
                        <i class="fa-regular fa-envelope me-1"></i>
                        <span>Superhit Top Movie </span>
                        <span class="txtColorPrimary">** King Star **</span>
                    </div>
                    <!-- Socials buttons -->
                    <div class="header-socials col-8">
                        <a class="text-reset " href=""><i class="fa-brands fa-facebook-f mx-2 facebook"></i></a>
                        <a class="text-reset " href=""> <i class="fa-brands fa-twitter mx-2 twitter"></i></a>
                        <a class="text-reset " href=""><i class="fa-brands fa-linkedin-in mx-2 linkedin"></i></a>
                        <a class="text-reset " href=""><i class="fa-brands fa-instagram mx-2 instagram"></i></a>
                        <a class="text-reset " href=""><i class="fa-brands fa-google-plus-g mx-2 google"></i></a>
                    </div>

                    <!-- Login -->
                    <div class="header-login col-1">
                        <a class="text-reset text-decoration-none" href="#">
                            <i class="fa-solid fa-lock me-2"></i>
                            <span>Login</span>
                        </a>
                    </div>
                </div>

            </div>
        </div>
        <!-- header search  -->
        <!-- header nav -->
    </div>
</template>

<script>
//  import HelloWorld from './HelloWorld.vue'

export default {
    name: 'AppHeader',
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
@use '../styles/partials/variables.scss';
@use '../styles/partials/_mixins.scss';

div.line {
    border-bottom: 1px solid #54595F;
}

.header-socials {

    i.facebook:hover,
    i.twitter:hover,
    i.linkedin:hover,
    i.instagram:hover,
    i.google:hover {
        color: #13be13;
    }

    i {
        transition: all .8s;
    }

    i.facebook {
        color: #3b5998;
    }

    i.twitter {
        color: #00acee;
    }

    i.linkedin {
        color: #0e76a8;
    }

    i.instagram {
        color: #c8232c;
    }

    i.google {
        color: #db4a39;
    }
}
</style> 
