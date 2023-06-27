<template>
    <div class="my_container">
        <nav class="mb-5">
            <ul class="list-unstyled d-flex">
                <li class="active" value="all">All</li>
                <li value="coming-soon"><span>Coming Soon</span></li>
                <li value="latest-movie"><span>Latest Movie</span></li>
                <li value="top-rating"><span>Top Rating</span></li>
                <li value="top-series"><span>TV Series</span></li>
            </ul>
        </nav>
    </div>
</template>

<script>

export default {
    name: 'MovieVideoContainers',
    props: {
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
@use '../../styles/partials/_variables.scss';
@use '../../styles/partials/_mixins.scss';
@use '../../styles/general.scss';

nav {
    height: 40px;

    ul {
        font-size: 18px;

        li {
            margin-right: 35px;
            cursor: pointer;
            transition: all .8s;
        }

        li:hover {
            color: #13be13;

            span:after {
                width: 100%;
            }
        }

        span:after {
            content: "";
            display: table;
            height: 5px;
            width: 0;
            border-bottom: 1px solid #13be13;
            transition: all .5s;
        }

    }
}

.active {
    color: #13be13;
}
</style> 

