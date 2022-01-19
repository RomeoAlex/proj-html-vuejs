<template>
    <div class="news-container">
        <img :src="require(`../assets/images/${details.image}`)" :alt="details.title">
            <div class="news-title">
                {{details.title}}
            </div>
            <div class="news-description">
                {{details.description}}
            </div>
    </div>
    
</template>
<script>

export default {
    name:'Newscard',
    props: {
        details: Object
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/general.scss';
@import '../assets/style/variables.scss';

.news-container{
    width: calc((100% / 2) - 40px);
    text-align: center;
    margin-right: 30px;
    img{
        max-width:100%;
    }
    .news-title{
        margin-top:15px;
        font-size:30px;
        font-weight: bold;
    }
    .news-description{
        margin-top:20px;
        font-size: 20px;
    }
    
}
</style>