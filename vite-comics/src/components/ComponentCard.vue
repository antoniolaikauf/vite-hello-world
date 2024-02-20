<script>

export default {
    name: "card",
// array contenete i dati da mettere dentro alla pagina 
    props: {
        cards: Array
    }
}
</script>

<template>
    <div v-for="(card, i) in cards" :key="i" class="card-iesima">
        <img :src="card.thumb" alt="">
        <div>
            {{ card.series.toUpperCase() }}
        </div>
    </div>
</template>

<style scoped lang="scss">
@use '../style/general.scss' as *;
@use '../style/partials/variable' as *;

// caratteristiche card 
.card-iesima {
    width: calc(100% / 6 - 10px);
    margin: 5px;
    font-size: 10px;

    img {
        width: 100%;
        height: 200px;
        object-fit:cover;
    }
}
</style>