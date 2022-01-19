<template>
<div class="sub-wrapper">
<h2>Stay in The Loop</h2>
<p>Sign up to receive up to date news and offers directly in your inbox:</p>
<input type="text" placeholder="your@email.com">
<!-- @click con funzione id invio dati -->
<button class="subscrive primary">SUBSCRIBE</button>
</div>
</template>

<script>
export default {
  name: "Subscribe",

};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import '../assets/style/general.scss';
@import '../assets/style/variables.scss';
.sub-wrapper{
    width:100%;
    margin: auto;
    text-align: center;
    color: white;
    h2{
        font-size: 50px ;
        padding:20px 0;
        color:$GoldenRod;
    }
    p{
       font-size: 20px ;
        padding:20px 0; 
    }
    input{
        width:600px;
        padding:10px;
        border-radius:25px;
        margin-bottom: 10px;
    }
    .subscrive{
        width:600px;
        padding:5px;
        border-radius:25px;
        display:block;
        margin: auto;
    }
}
</style>