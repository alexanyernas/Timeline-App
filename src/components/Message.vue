<template>
    <v-card
        class="mx-auto mb-6 my-card elevation-16"
    >   
        <v-img
            class="white--text align-end my-img"
            src="../assets/7-min.jpg"
            gradient="to bottom, rgba(0,0,0,0), rgba(0,0,0,.3)"
        >
            <v-card-title class="my-title justify-center">Te amo</v-card-title>
        </v-img>
    </v-card>
</template>

<script>
export default {
    name: 'Message'
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&display=swap');

.my-card
{
    max-width: 600px;
}

.my-img
{
    height: 500px;
}

.my-title
{
    font-family: 'Dancing Script', cursive; 
    font-size: 98px;
    margin-bottom: 36px;
}

.my-title::after
{
    content: '❤';
}

@media only screen and ( max-width: 600px ) 
{
    .my-card
    {
        max-width: 300px
    }

    .my-img
    {
        height: 250px;
    }

    .my-title
    {
        font-size: 48px;
        margin-bottom: 8px;
    }
}
</style>