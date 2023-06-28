<template>
    <div class="carousel-wrapper my_container container-fluid p-0 marginBottom">
        <div class="row d-flex ">
            <div v-for="movie in movieList" class="col-4 p-0 card_container">
                <MovieCard :movie=movie />
            </div>
        </div>
    </div>
</template>

<script>
import MovieCard from './NewMovieCard.vue'
export default {
    name: 'MovieCarousel',
    props: {
    },
    components: {
        MovieCard,
    },
    data() {
        return {
            index: '',
            movieList: [
                {
                    img: 'card-6.jpg',
                    title: 'Quisque auctor  Movie in Strack',
                    category: 'Coming Soon',
                    views: '1014',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '4',
                },
                {
                    img: 'card-10.jpg',
                    title: 'New Movie Quisque in Strack',
                    category: 'Latest Movie',
                    views: '748',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-3.jpg',
                    title: 'Movie Action Garila English',
                    category: 'Top Rating',
                    views: '376',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '1',
                },
                {
                    img: 'card-11.jpg',
                    title: 'Action Garila English Movie',
                    category: 'TV Series',
                    views: '305',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-12.jpg',
                    title: 'Donec English Action movie',
                    category: 'Coming Soon',
                    views: '492',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '10',
                },
                {
                    img: 'card-13.jpg',
                    title: 'English Action movie in Strack',
                    category: 'Latest Movie',
                    views: '280',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-14.jpg',
                    title: 'Movie Auctor Quisque in Strack',
                    category: 'Top Rating',
                    views: '306',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-15.jpg',
                    title: 'Movie Auctor Quisque in Strack',
                    category: 'TV Series',
                    views: '349',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '1',
                },
                {
                    img: 'card-16.jpg',
                    title: 'Movie Auctor Quisque in Strack',
                    category: 'Coming Soon',
                    views: '373',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '1',
                },
                {
                    img: 'card-6.jpg',
                    title: 'Movie Auctor Quisque in Strack',
                    category: 'Latest Movie',
                    views: '511',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-5.jpg',
                    title: 'Movie Auctor Quisque in Strack',
                    category: 'Top Rating',
                    views: '354',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '1',
                },
                {
                    img: 'card-4.jpg',
                    title: 'Nulla Strack New Animate Movie',
                    category: 'TV Series',
                    views: '342',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-3.jpg',
                    title: 'Blue Strack New Animate Movie',
                    category: 'Coming Soon',
                    views: '428',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-2.jpg',
                    title: 'Animate Blue Strack New Movie',
                    category: 'Latest Movie',
                    views: '367',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
                {
                    img: 'card-2.jpg',
                    title: 'Hurry Animate Blue Strack New Movie',
                    category: 'Top Rating',
                    views: '429',
                    release: 'February 12, 2016',
                    genre: 'Drama, Action Releas',
                    rating: '0',
                },
            ]
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

.card_container {
    border-radius: 25px;
    overflow: hidden;
}
</style> 

