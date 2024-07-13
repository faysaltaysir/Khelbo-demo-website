<template>
        <section class="image-section">
            <div class="image-container">
                <img src="../assets/image.png" alt="">
                <div class="text-overlay">
                    <div class="writings">
                        <p class="racing-sans-one-regular head">Own a Turf!</p>
                        <p class="racing-sans-one-regular secound-text">Get Register Today</p>
                    </div>
                    <div class="register ">
                        <button></button>
                        <p class="text poppins-thick">Register Your Turf!</p>
                    </div>
                </div>
            </div>
        </section>
</template>

<script>

</script>
<style scoped>
.news-letter{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    
}
.secound-text{
    position: relative;
    left: 8vw;
    bottom: 1vw;
    font-size: 1.7vw;
    
}
    .register{
        width: 50%;
        display: flex;
        justify-content: center;
    }
    img{
        width: 100%;
        /* height: 388px; */
    }
    .image-section{
        position: relative;
        width: 100%;
    }
    .image-container{
        position: relative;

    }
    .text-overlay{
        width: 100vw;
        position: relative;
        bottom: 14vw;
        display: flex;
        justify-content: space-around;
        align-items: center;
        color: white;
    }
    .head{
        font-size: 4vw;
        background-color: #09ec14;

    }

    
    .writings{
        position: absolute;
        right: 50%;
        padding-right: 10vw;
        line-height: 0.01vw;
    }
    button{
        width: 29vw;
        height: 6vw;
        border: 0px;
        border-radius: 2vw;
        background-image: linear-gradient(to bottom, #FF0202, #990101); 
        color: white;
        transform: skew(-20deg);
        margin-right: 10vw;
    }
    .register{
        position: absolute;
        left: 50vw;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    .text{
        position: absolute;
        font-size: 2vw;
        margin-right: 10vw;
        /* font-weight: 600; */
        /* right: 160px; */
    }

</style>