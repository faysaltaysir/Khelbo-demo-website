<template> 

    <div class="body">        
        <h1 class="headings poppins-thick">Our Popular Venues</h1>
        
        <div class="slider poppins-thick">
            <div v-for="card of cards" class="slide-track" :key="card.id">
                <div class="card">
                    <img src="../assets/gnd_1.png" alt="ground_1">
                    <div class="contents poppins-thin">
                        <div class="featured">Featured</div>
                        <div class="discount">
                            <p class="percentage poppins-thick">{{ card.percentage }}</p>
                            <p class="discount-text">Discount</p>
                        </div>
                        <div class="rating poppins-thick">
                            <div class="left">
                                <p>{{ card.rating }}</p>
                                <p class="review poppins-thin">({{ card.review }} review)</p>
                            </div>
                            <div class="right">
                                <p class="vs poppins-thin drop-shadow">{{ card.vs }}</p>
                                <img class="icon" src="../assets/football.png" alt="">
                            </div>
                        </div>
                        
                    </div>
                    
                    <div class="writing">
                        <p class="title">{{ card.title }}</p>
                        <p class="para">
                            <span class="material-symbols-outlined">location_on</span>
                            {{ card.location }}</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="space">
        <hr>
    </div>
</template>

<script>
    export default{
        data(){
            return{
                cards: [
                    {   id: 1,
                        title: "Oxygen Sports Turf",
                        location: "Pered Math, College Road, Chittagong",
                        image: "../assets/gnd_1up.png",
                        percentage: '50%',
                        rating: '4.95',
                        review: '234',
                        vs: '7vs7',
                    },
                    {
                        id: 2,
                        title: "Victory Sports Arenca",
                        location: "Pered Math, College Road, Chittagong",
                        percentage: '30%',
                        rating: '4.95',
                        review: '234',
                        vs: '7vs7',
                    },
                    {
                        id: 3,
                        title: "Lohagara Turf",
                        location: "Pered Math, College Road, Chittagong",
                        percentage: '20%',
                        rating: '4.95',
                        review: '234',
                        vs: '7vs7',
                    },

                    
                ]
            }
        }
    }
</script>

<style scoped>
.writing{
    padding-left: 1vw;
    position: relative;
    bottom: 15px;
    
}
.title{
    font-size: 20rem;
    color: red;
}
.para{
    position: relative;
    bottom: 15px;
    display: flex;
    align-items: center;
    font-size: 1vw;
}
.space{
    margin-left: 1vw;
    margin-right: 1vw;
    /* height: 2px; */
    margin-top: 1vh;
    margin-bottom: 10vh;
    padding-left: 10vw;
    padding-right: 10vw;
}
.line{
    /* width: 80%; */
    height: 0px;
    border-top: 0px;
    border-color: #474954;
    border-block-style: solid;
    /* margin: 50px 150px 50px 150px; */
    
}
.headings{
    margin-top: 50px;
    /* display: block; */
    /* margin-left: 10vw; */
    /* margin-right: 10vw; */
}
.title{
    font-size: 1.2rem;
    font-weight: 400;
}
.writing{
    line-height: 1rem;
}
.writing .para{
    color: rgb(96, 96, 96);
}
    .body {
            /* display: flex; */
            /* justify-content: center; */
            /* align-items: center; */
            height: fit-content;
            /* margin: 0; */
            /* background-color: #e20000; */
            overflow: hidden; /* Prevent scrolling */
            margin-left: 10vw;
            margin-right: 10vw;
        }

    .card{
        position: relative;
        max-width: 500px;
        max-height: 500px;
        width: 40vw;
        height: 40vw;
        padding: 1vw;
        display: flex;
        flex-direction: column;
        margin-left: 1vw;
        margin-right: 1vw;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
        overflow: hidden;
        cursor: pointer;
        border-radius: 20px;
        /* box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); */
    }
    .card:hover {
        transform: scale(1.05);
        box-shadow: 0 16px 16px rgba(0, 0, 0, 0.2);
    }

    img{
        width: 100%;
        border-radius: 10px;
        /* max-width: 470px; */
    }

 

        .slider {
            min-height: 300px;
            max-height: 500px;
            height: 40vw;
            display: flex;
            overflow: hidden;
            width: 100%;
            /* max-width: 1300px; */
        }

        .slide-track {
            display: flex;
            animation: scroll 3s linear infinite;
            
        }
        .contents{
            
            width: 100%;
            height: 100%;
            position: absolute;
            color: white;
            /* font-size: 5vh; */
            /* padding-left: 2px; */
        }
        .featured{
            width: 35%;
            /* height: 10%; */
            /* max-width: 100px; */
            /* max-height: 25px; */
            padding: 2px;
            background-color: #EC7304;
            position: absolute;
            top: 10%;
        }
        .discount{
            position: relative;
            width: 15vw;
            height: 10vh;
            min-height: 40px;
            max-height: 6vh;
            /* padding: 2px; */
            background-color: #EC0404;
            /* position: absolute; */
            top: 20%;
            /* display: flex; */
            /* justify-content: center; */
            /* flex-direction: column; */
            /* align-items: center; */
            line-height: 1px;
            /* padding-bottom: 10px; */
            font-size: 1rem;
        }
        .percentage{
            padding-top: 10px;
            text-align: center;
        }
        .discount-text{
            text-align: center;
        }
        
        
        .rating{
            width: 100%;
            position: absolute;
            top: 55%;
            /* padding-right: 10%; */
            display: flex;
            justify-content: space-between;
            align-items: center;
            /* padding-left: 1vw; */
            /* margin-right: 10px; */
            /* background-color: #EC0404; */
            /* -webkit-text-stroke: .1px rgb(255, 255, 255);  */
            font-size: 1.3vw;
        }
        .review{
           
            font-weight: 300;
        }
        .vs{
            border: 1px solid white;
            border-radius: 5vw;
            margin-right: 1vw;
            font-size: 1.1vw;
            /* stroke-width: 4rem; */
            font-weight: 400;
            
            /* padding: 20px; */
            padding-left: 1vw;
            padding-right: 1vw;
            
            -webkit-text-stroke: .1px #D9D9D9;
        }
        .drop-shadow {
           text-shadow: 
            2px 2px 5px rgba(0, 0, 0, 0.7), 
            4px 4px 10px rgba(0, 0, 0, 0.5);
    }
        .icon{
            height: 3vw;
            width: 3vw;
        }
        .left{
            display:flex ;
            padding-left: 1vw;
            text-overflow: clip;
        }
        .right{
            display: flex;
            align-items: center;
            padding-right: 4vw;
        }
        
       
        @keyframes scroll {
            0% {
                transform: translateX(0);
            }
            100% {
                transform: translateX(calc(-100px * 3)); /* Adjust according to the number of cards */
            }
        }

        /* Media Queries */
        @media (max-width: 600px) {
            .card {
                min-width: 200px;
                min-height: 200px;
            }
            .title{
                font-size: 1rem;
            }
        }
</style>