<template>
    <div class="wrapper">
        <div class="my_jumbo"></div>
        <div class="texts-container">
            Coming Soon Movie
            <h1>Max Still</h1>

            jon player & Emily Rose

            The countdown is finished!
        </div>
    </div>
</template>

<script>

export default {
    name: 'Jumbo',
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

div.wrapper {
    position: relative;
}

div.texts-container {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    left: 50%;
    padding: 30px;
}

div.my_jumbo {
    background-color: aqua;
    height: 650px;
    background-image: url(../../../public/coming-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    opacity: .5;
    margin-bottom: 90px;

}
</style> 
