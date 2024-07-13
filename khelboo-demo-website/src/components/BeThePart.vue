<template>
    <div class="body">
        <div class="left">
            <img class="left-img" src="../assets/be-the-part.png" alt="be-the-part">
        </div>
        <div class="right">
            <div class="img1-out">
                <img class="img1" src="../assets/21.png" alt="">
                <p class="img1-para poppins-thick">Create A Team</p>
            </div>
            <div class="img2-out">
                <img class="img2" src="../assets/12.png" alt="">
                <p class="img1-para poppins-thick">Challenge A Team</p>
            </div>
            </div>
        </div>    
</template>
<script>

</script>
<style scoped>
.img1-para{
    max-width: 40%;
    width: 60%;
    flex-wrap: wrap;
    position: absolute;
    bottom: -12px;
    font-size: 3vw;
}
.img2-para{
    max-width: 60%;
    width: 60%;
    flex-wrap: wrap;
    position: absolute;
    top: 0px;
    font-size: 1rem;
}
.img1-out{
    /* width: 45vw; */
    height: 100%;
    position: relative;
    /* bottom: 6vw; */
}
.img2-out{
    position: relative;
    width: 49vw;
    height: 100%;
}
.img2{
    width: 4vw;
}


.body{
    width: 100vw;
    height: 100%;
    position: relative;
    top: 100px;
    display: flex;
    align-items: center;
    margin: 5vw 10vw 5vw 10vw;
    /* justify-content: space-between; */
}
.left{
    width: 50%;
    height: 100%;
    /* background-color: blue; */
    margin-right: 6vw;
    
}
.left-img{
    height: 100%;
    width: 100%;
}
.right{
    width: 50%;
    position: relative;
    display: flex;
    justify-content: center;
    flex-direction: column;
    /* margin-left: 2px; */
}


.right img{
    width: 76%;
    position: relative;
    right: 10vw;
    padding-left: 5vw;
    /* border: 1px solid black; */
}

</style>
