<template>
    <div class="class ">
        <img src="../assets/image.png" alt="">
        <div class="contents">
            <div class="writings">
                <p class="racing-sans-one-regular head">Own a Turf!</p>
                <h2 class="racing-sans-one-regular secound-text">Get Register Today</h2>
            </div>
            <div class="register ">
                <button class="poppins-thin">Register Your Turf</button>
            </div>
        </div>
        <div class="newsletter ">
            <h1>Join Our NEWSLETTER</h1>
            <p>Get Offers and New Updates to keep up uour sport sprits</p>
        </div>
        
    </div>    
</template>

<script>

</script>
<style scoped>
.newsletter{
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    

}
    .secound-text{
        position: relative;
        bottom: 5vw;
        left: 7vw;
        font-size: 2vw;
    }
    .head{
        font-size: 4vw;
    }
  
    img{
        width: 100%;
        /* position: relative; */
        /* margin: 0px;   */
    }
    .contents{
        position: absolute;
        top: 160%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: flex;
        justify-content: space-around;
        align-items: center;
        color: #FAFAFA;
        
    }
    .racing-sans-one-regular {
        font-family: "Racing Sans One", sans-serif;
        font-weight: 900;
        font-style: bold;
    }

    button{
        width: 26vw;
        height: 5vw;
        border: 0px;
        border-radius: 10px;
        background-image: linear-gradient(to bottom, #FF0202, #990101); 
        color: white;
        transform: skew(20deg);
        font-style: normal;
        font-weight: 100;
    }
    /* .poppins-thin {
        font-family: "Poppins", sans-serif;
        font-weight: 100;
        font-style: normal;
        font-size: 1.9vw;
    } */
</style>