<template>
        <!-- da rivedere -->
        <a class="food-card-container" :href="details.url">
            <div class="food-single-card">
                <span class="food-categories-name">{{details.name}}</span>
                <img :src="require(`../assets/images/${details.image}`)" :alt="details.name">
            </div>
        </a>
            
    
</template>
<script>

export default {
    name:'FoodCategoriesCard',
    props: {
        details: Object
    },
}
</script>

<style lang="scss" scoped>
@import '../assets/style/general.scss';
@import '../assets/style/variables.scss';


    
    .food-card-container{
        width: calc((100% / 4) - 30px );
        margin-bottom: 10px;
        margin-right: 10px;
    .food-single-card{
                position: relative;
                span{
                        font-size: 18px;
                        color:white;
                    }  
                .food-categories-name{
                    position: absolute;
                    top: 50%;
                    left: 50%;
                    transform: translate(-50%, -50%);
                    z-index: 2;
                               
    }
    img{
        max-width:100%;
        
    }
    }
    }
</style>