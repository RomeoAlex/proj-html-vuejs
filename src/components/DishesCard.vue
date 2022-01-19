<template>
    <div class="dishes-container">
        <img :src="require(`../assets/images/${details.image}`)" :alt="details.name">
            <div class="dishes-name">
                {{details.name}}
            </div>
            <div class="dishes-price">
                {{details.price}}
            </div>

    </div>
    
</template>
<script>

export default {
    name:'DishesCard',
    props: {
        details: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/general.scss';
@import '../assets/style/variables.scss';

.dishes-container{
    width: calc((100% / 3) - 15px);
    min-height: 400px;
    padding: 30px;
    text-align: center;
    margin-bottom: 20px;
    margin-right:15px;
    img{
        max-width:100%;
    }
    .dishes-name{
        margin-top:15px;
        font-size:30px;
    }
    .dishes-price{
        margin-top:20px;
        font-size: 20px;
        color:$RedCardinal;
    }
    
}
</style>