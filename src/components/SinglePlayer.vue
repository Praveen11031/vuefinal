<template>
    <div>

        <p v-if="player">Name:  {{ player.Name }}</p>
        <p v-if="player">Currentteam:  {{ player.Current }}</p>
        <p v-if="player">DateOfBirth:  {{ player.Dob }}</p>
        <p v-if="player">AvalableforAuction:  {{ player.Available }}</p>
        <p v-if="player">MinimumBiddingprice:  {{ player.Minimumbid }}</p>

                     
    </div>
</template>

<script>

export default{
    name: 'SinglePlayer',
    props:{
        player: Array
    }
}
</script>

<style scoped>

.green{
    background-color: rgb(77, 143, 77);
}

h4{
    margin: 2px;
}

div{
    background-color: #b48c7e;
    color: black;
    padding: 1em;
    text-align: center;
    width: 80%;
    margin: auto;
    

}

.red{
background-color: orangered !important;

}


</style>