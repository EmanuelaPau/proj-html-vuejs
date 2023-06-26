<template>
    <footer class="">
        <!-- About Us  -->
        <div class=" ">
            <div class="container-fluid footer-about">
                <div class="row my_container">
                    <div class="col-3 px-3">
                        <h1 class="my_h1">
                            About Us
                        </h1>
                        <p class="my_p">
                            Mauris malesuada arcu eu posuere eleifen. Ut egestas tortor at leo egestas tincidunt. Nam
                            tincidunt metus tristique tristique viverra. Mauris erat ante, egestas vitae dapibus seds.
                        </p>
                        <ul class="list-unstyled d-flex flex-wrap">
                            <li v-for="icon in    socialIcons   " class="me-3 social-icon">
                                <a :class="icon" href="">
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3 px-3">
                        <h1 class="my_h1">
                            Movie Category
                        </h1>
                        <ul class="list-unstyled">
                            <li v-for="li in movieCategory" class="footer-li">
                                <a class="text-decoration-none text-reset" href="">{{ li.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3 px-3">
                        <h1 class="my_h1">
                            Information
                        </h1>
                        <ul class="list-unstyled">
                            <li v-for="li in information" class="footer-li">
                                <a class="text-decoration-none text-reset" href="">{{ li.name }}</a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3 px-3">
                        <h1 class="my_h1">
                            Recent Posts
                        </h1>
                        <div v-for="cards in recentPosts" class="footer-card d-flex">
                            <img :src="cards.img" alt="">
                            <div class="d-flex flex-wrap align-items-end">
                                <p class="my_p m-0">{{ cards.title }}</p>
                                <p class="my_p m-0">{{ cards.date }}</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

        </div>
        <div class="footer-about-back"></div>
        <!-- Footer bottom  -->
        <div class="container-fluid">
            <div class="row my_container py-3">
                <div class="col-6">
                    <ul class="d-flex flex-wrap list-unstyled my_nav m-0">
                        <li v-for="   element    in    footerBottomNav   " class="me-4">
                            <a class="text-reset text-decoration-none" href="">
                                {{ element }}
                            </a>
                        </li>

                    </ul>
                </div>
                <div class="col-6 d-flex flex-wrap justify-content-end px-0">
                    <span class="me-1">
                        © 2020
                    </span>
                    <span class="txtColorPrimary me-1 my_info">
                        <a class="" href="">@Themepul</a>
                    </span>
                    <span>
                        All Rights Reserved.
                    </span>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>

export default {
    name: 'AppFooter',
    props: {
        aboutUs: 'Object',
        movieCategory: 'Object',
        information: 'Object',
        recentPosts: 'Object',
        footerBottomNav: 'Object',
        socialIcons: 'Array',
    },
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

.footer-about {
    padding-top: 70px;
    height: 500px;
    width: 100%;
    line-height: 24px;

    position: absolute;
    left: 0;
}

.footer-li {
    height: 48px;
    font-size: 15px;
}

.footer-card {
    width: 100%;
    height: 85px;
    margin-bottom: 30px;

    img {
        height: 100%;
        margin-right: 10px;
    }


}

div.footer-about-back {
    height: 500px;
    background-image: url('../../public/ft-bg.jpg');
    background-size: cover;
    background-position: center;
    filter: grayscale(100%);
    opacity: 0.1;

    position: relative;
}


.my_nav li a {
    transition: all .8s;
}

.my_nav li a:hover {
    color: #13be13;
}

.my_info a {
    transition: all .8s;
    color: #13be13;
}

.my_info a:hover {
    color: white;
}

h1.my_h1 {
    font-size: 18px;
    margin-bottom: 30px;
}

p.my_p {
    font-size: 14px;
}

.social-icon {
    height: 32px;
    width: 32px;
    border-radius: 50%;

    display: flex;
    align-items: center;
    justify-content: center;

    a {
        color: white;
    }
}
</style> 
