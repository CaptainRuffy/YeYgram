<template>
    <div class="wrap">
        <div class="container">
            <div id="square" :style="[{background: 'url(' + post.authorAvatarUrl + ')'}, {'background-size' : 'cover'}]"></div>
            <div>{{post.authorname}}</div>
        </div>
   
        <img :src="post.postpictureUrl" width="1000px">
    </div>
</template>

<script>
import Vue from "vue";


    export default Vue.extend({
        props: ['post']
    });


</script>

<style>
    #square {
    width: 100px;
    height: 100px;
    border-radius: 50%; 
    margin-bottom: 10px;
    margin-right: 10px;

}
.container{
    display: flex;
    align-items: center;
    font-size: 26px;
  
}
.wrap{
    width:1000px;
    margin: auto;
}
</style>