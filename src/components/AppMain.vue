<template>
    <main>
        <MainJumbo />
        <MainTitle :title=titles.newMovie.title :subtitle=titles.newMovie.subtitle />
        <MainMail />
    </main>
</template>

<script>
//  import HelloWorld from './HelloWorld.vue'
import MainJumbo from './Main/MainJumbo.vue'
import MainMail from './Main/MainMail.vue'
import MainTitle from './Main/MainTitle.vue'
export default {
    name: 'AppMain',
    components: {
        MainMail,
        MainJumbo,
        MainTitle,
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
