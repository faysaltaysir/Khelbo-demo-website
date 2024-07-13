<template>
    <div class="border poppins-thin">
        <hr>
        <h1>Explore Turfs Nearby You</h1>
    </div>
   
    <div class="outer-div">
        
            <span class="material-symbols-outlined">search</span>
            <input type="text" placeholder="Turf name" class="poppins-thick">
      
         
            <span class="material-symbols-outlined">location_on</span>
            <input type="text" placeholder="Location" class="poppins-thick">
        
        
            <span class="material-symbols-outlined">surfing</span>
            <input type="text" placeholder="Sports" class="poppins-thick">
      
        <button class="poppins-thick">Search</button>

    </div>
    <div class="border">
        <hr>
    </div>
</template>

<style scoped>
    
     .border{
        margin-top: 150px;
        margin-left: 10vw;
        margin-right: 1vw;
        margin-bottom: 2vw;
     }
    .material-symbols-outlined{
        position: relative;
        left: 32px;
        color:#D9D9D9;
        font-size: 1.5rem;
        /* padding-left:  */
    }
    button{
        color: white;
        background-image: linear-gradient(to bottom, #DD0007, #960005); 
        border: 0px;
        border-radius: 30vw;
        width: 6rem;
        height: 2rem;
        margin-right: 1vw;
        margin-left: 1vw;
        transition: font-size 0.3s ease;
    }
    button:hover{
        /* background-image: linear-gradient(to bottom, #0d0048, #00064c);  */
        /* color: rgb(235, 235, 235); */
        font-size: 1.02rem;
        text-decoration: underline;
        cursor: pointer;
    }
    input{
        width: 15vw;
        height: 2rem;
        border-radius: 1vh;
        border: 0px solid black;
        background-color: #F0F0F0;
        margin: 0.3vw;
        padding-left: 3vw;
    }
    input::placeholder {
        color: #D9D9D9;
        transition: color 0.3s ease;
    }

    /* input:focus { 
        border-color: #ff5050; 
        outline: none; 
    } */
    input:focus::placeholder {
        color: rgb(255, 133, 133);
    }

    .outer-div{
        width: 100%;
        /* min-width: 470px; */
        max-width: 1500px;
        position: relative;
        display: flex;
        flex: 1 1 10%;
        align-items: center;
        /* justify-content: center; */
        flex-direction: row;
        margin-left:10%;
        margin-right:10%;
        width: 80vw;
        height: 80px;
        background-color: #D9D9D9;
        justify-content: space-between;
        /* padding: 0x 10% 0px 10%; */
        border-radius: 10px;
    }

    @media screen and (max-width: 600px) {
        
        input{
            width: 20%;
            margin: 0.1vw;
            padding-left: 2rem;
        }
        button{
            width: 4rem;
            height: 2rem;
            margin-right: 10px;
            margin-left: 5px;
            transition: font-size 0.3s ease;
        }
        .material-symbols-outlined{ 
             visibility: hidden; 
         }
        .outer-div{
            margin: 5%;
        }
        .border{
            margin-left: 5%;
            margin-right: 5%;
        }
    } 

     @media screen and (max-width: 500px) {
        
        input{
            width: 20%;
            margin: 0.1vw;
            padding-left: 2rem;
        }
        button{
            width: 4rem;
            height: 2rem;
            margin-right: 10px;
            margin-left: 5px;
            transition: font-size 0.3s ease;
        }
        .material-symbols-outlined{ 
             visibility: hidden; 
         }
        .outer-div{
            margin: 5%;
        }
        .border{
            margin-left: 5%;
            margin-right: 5%;
        }
    } 
</style>