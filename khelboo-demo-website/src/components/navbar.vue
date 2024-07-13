<template>
    <div class="navbar poppins-thin ">
        <div class="screw"></div>

        <div class="left">
            <img class="logo" src="/src/assets/logo-main.png" alt="">
        </div>
        <div class="middle">
            
        <div class="section txt-hover" v-for="section of sections" :key="section.key">{{ section.name }}</div>
            
        </div>
        <div class="right">
           <button class="login poppins-thick txt-hover">Login</button> 
           <button class="signup poppins-thick">Signup</button>
            
        </div>
    </div>
</template>
<script>
import Input from './Input.vue'
    export default{
        components:{Input},
        props:['sections','sections2'],
        data(){
            return{
                placeHolder: 'Search',
            }
        }
    }
</script>
<style scoped>
    .txt-hover{
        transition: font-size 0.2s ease;
        cursor: pointer;
    }
    .txt-hover:hover{
        text-decoration: underline;
        font-size: 0.85rem;
    }
    .screw{
        position: absolute;
        width: 61px;
        height: 65px;
        margin-left: 90px;
        transform: skew(-20deg);
        background-color: white;
    }
    button{
        margin: 1vw;
    }
    .login{
        background-color: transparent;
        border: 0px;
        color: white;

    }
    .signup{
        width: 5rem;
        height: 2rem;
        border: 0px;
        border-radius: 10px;
        color: #C20B11;
        font-weight: bold;
        transition: font-size 0.3s ease;
    }
    .signup:hover{
        font-size: 1.01rem;

    }
    .left{
        width: 10%;
        display: flex;
        align-items: center;
        margin-left: 50px;
    }
    .navbar{
        position: absolute;
        left: 0px;
        top: 0px;
        width: 100vw;
        height: 60px;
        background-image: linear-gradient(to bottom, #DD0007, #9F0C10); 
        margin: 0px;
        display: flex;
    }
    .logo{
        position: absolute;
        top: 0px;
        width: 65px;
        height: 65px;
        left: 85px;
    }
    .middle{
        width: 60%;
        display: flex;
        align-items: center;
        justify-content: left;
        /* padding-left: 25px; */
    }
    .right{
        width: 25vw;
        border-left: 2px solid white;
        margin-top:10px;
        margin-bottom:10px;
        padding-left: 1vw ;
        display: flex;
        align-items: center;
        justify-content: left;
        padding-right: 1vw;
    }
    .section{
        width: 60%;
        height: 50px;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 0px 0.01vw 0px 0.01vw;
        cursor: pointer;
        color: white; 
        font-size: .8rem;
    }
    
    .extra:hover{
        height: 30px;
        background-color: rgba(170, 90, 255, 0.1);
        color: black;
        border-radius: 20px;
        
    }
    
    .extras:hover{
        background-color: rgba(170, 90, 255, 0.4);
        color: black;
        border-radius: 20px;
        
    }
    
    .person{
        color: rgb(0, 148, 148);
        border: 4px solid rgb(209, 249, 254);
        border-radius: 50%;
        padding: 3px;
        margin: 10px;
        font-size: 30px;
    }
    .blank{
        width: 20%;
    }
    @media screen and (max-width: 880px) {
        .section{
            padding: 0px 5px 0px 5px;
            visibility: hidden;
        }
        .right{
            margin-right: 1vw;
        }
        
        
    }
    @media screen and (max-width: 650px) {
        .section{
            visibility: hidden;
            width: 5%;
            
        }
        .right{
            /* width: 100%; */
            margin-right: 50px;
        }
    }
    @media screen and (max-width: 445px) {
        
        .right{
            position: absolute;
            right: 10vw;
            border: 0px;
        }
    }

    
    

</style>