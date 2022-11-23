<script>

export default{

 name : 'Circle', 

  data(){
    return{
        message : "ciao"
    }
  }
}



</script>

<template>


<div class="container">

    <div class="box">
        <div class="circle">95%</div>
        <svg height="300" width="300">
          <circle cx="150" cy="150" r="97" stroke="red" stroke-width="8px" fill="none" />
       </svg>
    </div>

</div>


</template>

<style lang="scss" scoped>

.container{
    display: flex;
    justify-content: center;
    padding: 1rem;

    img{
        max-width: 100%;
    }

.box{
    display: flex;
   justify-content: center;
   align-items: center;
   position: relative;
   height: 500px;
   width: 500px;
   background-color: greenyellow;

.circle{
    height: 200px; 
    width: 200px; 
    border-radius: 50%;
    border: 8px solid lightpink; 
    background-color: lightgreen;
    display: flex;
    justify-content: center;
    align-items: center;
   
}
svg{
        position: absolute;
        transform: rotate(-90deg);
        
        circle{
            stroke-dashoffset: 30;
            stroke-dasharray: 609;
        }
    }
}
}

</style>