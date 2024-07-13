<template>
    <div class="border">
        <div class="rectangles">
           <div class="left">
            <div class="div1"></div>   <!--done-->
           </div>
           <div class="right">
                <div class="div2">
                    <!-- <div class="div-new"></div>  done -->
                </div>  <!--done-->
                
                <div class="div3"></div>  done
           </div>
           
        </div> 
        <div class="line"></div>
        <h1>Explore Turfs Nearby You</h1>
    </div>
    
</template>
<style scoped>

.div-new{
    width: 200px;
    height: inherit;
    position: relative;
    right: 20px;
    transform: skew(-20deg);
    /* transform: skewX(50deg); */
    background-color: black;
}

.div1{
    width: 500px;
    height: 320px;
    background-color: brown;
    /* margin: 20px; */
    /* transform: skew(-20deg); */
    border-radius: 30px;
}
.div2{
    /* transform: skew(-20deg); */
    /* margin: 20px; */
    /* margin-left: 50px; */
    position: relative;
    /* left: 50px; */
    border-radius: 30px;
    width: 555px;
    height: 150px;
    background-color: rgb(8, 15, 226);
    /* margin: 20px; */
    /* transform: skew(-20deg); */
    
}

.div3{
    /* transform: skew(-20deg); */
    /* margin: 20px; */
    /* margin-left: 50px; */
    /* position: relative; */
    /* left: 50px; */
    border-radius: 30px;
    position: relative;
    /* right: 55px; */
    width: 555px;
    height: 150px;
    background-color: rgb(1, 111, 74);
    /* margin: 20px; */
}
.right{
   display: flex;
   flex-direction: column;
   justify-content: right;
   background-color: brown;
   /* margin: 30px; */
}
.line{
    width: 90%;
    height: 0px;
    border-top: 1px;
    border-color: #474954;
    border-block-style: solid;
    margin: 50px 0px 50px 0px;
    
}
.border{
    background-color: aqua;
    display: flex;
    flex-direction: column;
    margin-left: 150px;
    margin-right: 150px;
    /* width: 100%; */
    /* align-items: center; */
}

.rectangles{
    padding-top: 50px;
    height: 300px;
    /* width: 100%; */
    margin: 200px 0px 0px 0px;
    background-color: rgb(226, 168, 43);
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    
}
    .body{
        position: absolute;
        width: 100%;
        height: 100vh;
        top: 61px;
        left: 0px;
        background-color: #ffffff;
        color: white;
        padding: 10px;
    }
    .heading{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0px 100px 0px 100px;
        
    }
    .sub-body{
        margin:25px 100px 25px 100px;
    }
    .inp-size{
        width: 15rem;
        height: 2.2rem;
        background-color: #474954;
        color: white;        
    }
</style>
<script>
import Input from './Input.vue'
    export default{
        components:{Input},
        data(){
            return{
                placeHolder: 'Filter..'
            }
        }
    }
</script>