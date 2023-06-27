<template>
    <main>
        <MainJumbo />
        <MainTitle :title=titles.newMovie.title :subtitle=titles.newMovie.subtitle />
        <MainTitle :title=titles.moviePlaylist.title :subtitle=titles.moviePlaylist.subtitle />
        <MainTitle :title=titles.newMovie.title :subtitle=titles.newMovie.subtitle />
        <MainTitle :title=titles.latestNews.title :subtitle=titles.latestNews.subtitle />
        <SquareCardsContainer :bigCardName=squareCards.big.title :bigCardImg=squareCards.big.img
            :bigCardFont=squareCards.big.fontSize :bigCardDate="squareCards.big.date"
            :bigCardDisplay="squareCards.big.display" :smallCard=squareCards.small />
        <MainMail />
    </main>
</template>

<script>
//  import HelloWorld from './HelloWorld.vue'
import MainJumbo from './Main/MainJumbo.vue'
import MainMail from './Main/MainMail.vue'
import MainTitle from './Main/MainTitle.vue'
import SquareCardsContainer from './Main/MainSquareCardsContainer.vue'
export default {
    name: 'AppMain',
    components: {
        MainMail,
        MainJumbo,
        MainTitle,
        SquareCardsContainer,
    },
    data() {
        return {
            titles: {
                newMovie: {
                    title: 'New Movie',
                    subtitle: 'Lorem Ipsum is simply dummy text of the printing and typesettin',
                },
                moviePlaylist: {
                    title: 'Movie Playlist',
                    subtitle: 'Lorem Ipsum is simply dummy text of the printing and typesettin',
                },
                latestNews: {
                    title: 'Latest News',
                    subtitle: 'Lorem Ipsum is simply dummy text of the printing and typesettin',
                }
            },
            squareCards: {
                big: {
                    title: 'Actor The Concept Movie High Concept Theory see the post',
                    img: 'blog-570x570.jpg',
                    fontSize: 'my_h1-big',
                    date: '14 April, 2020',
                    display: ''
                },
                small: [
                    {
                        title: 'consequat Nam lectus nibh aucibus It has turpis',
                        img: 'blog2-570x570.jpg',
                        fontSize: 'my_h1-small',
                        date: '14 April, 2020',
                        display: 'd-none'
                    },
                    {
                        title: 'consequat Nam lectus nibh aucibus It has turpis',
                        img: 'blog3-570x570.jpg',
                        fontSize: 'my_h1-small',
                        date: '14 April, 2020',
                        display: 'd-none'
                    },
                    {
                        title: 'consequat Nam lectus nibh aucibus It has turpis',
                        img: 'blog4-570x570.jpg',
                        fontSize: 'my_h1-small',
                        date: '14 April, 2020',
                        display: 'd-none'
                    },
                    {
                        title: 'consequat Nam lectus nibh aucibus It has turpis',
                        img: 'blog5-570x570.jpg',
                        fontSize: 'my_h1-small',
                        date: '14 April, 2020',
                        display: 'd-none'
                    },
                ]
            }
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
