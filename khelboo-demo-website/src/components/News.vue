<template>
    <div class="body">
        <!-- <div class="body-inside"> -->
            <div class="writing ">
                <div class="txt-total">
                    <P class="heading poppins-thick">Join Our NEWSLETTER</P>
                    <P class="text poppins-thin">Get Offers and New Updates to keep up uour sport sprits</P>
                </div>
                <div class="input">
                    <input class="poppins-thin" type="text" name="" id="" placeholder="Your Mail">
                    <button class="poppins-thin">Subscribe</button>
                </div> 
            </div>
        <!-- </div> -->
    </div>
</template>
<style scoped>
.txt-total{
    height: 90px;
}
.text{
    position: relative;
    bottom: 25px;
}
    .body{
        height: 130px;
        display: flex;
        justify-content: center;
    }

    .writing{
        min-width: 350px;
        width: 50vw;
        display: flex;
        flex-direction: column;
        text-align: center;
        line-height: 25px;
        
    }
    .heading{
        font-size: 1.6rem;
        font-weight: 500;
    }
    
    .text{
        font-size: 1rem;
        
    }
    .input{
        min-width: 340px;
        position: relative;
        top: 20px;
    }


    input{
        min-width: 170px;
        width: 30vw;
        height: 40px;
        border: 0;
        border-top-left-radius: 10px;
        border-bottom-left-radius: 10px;
        padding-left: 20px;
        background-color: rgb(239, 239, 239);
    }
    button{
        min-width: 75px;
        width: 10vw;
        height: 43px;
        border: 0px;
        background-image: linear-gradient(to bottom, #AE0404, #DC0007); 
        color: white;
        border-top-right-radius: 10px;
        border-bottom-right-radius: 10px;
    }
    
</style>