<template>
    <div class="container mb-12 w-full mt-16">
      <div class="moving-element flex justify-between">
        <li class="flex justify-between group gap-[200px] list-none bg-[#0d0d12]">
            <ul class="w-[260px]">
        <Card 
          href="https://instagram.com/ethkopa"
          title="Daniel Kopa"
          role="CEO and Founder"
          body="Stoked For this!"
          image="https://cdn.discordapp.com/avatars/886919873693888523/59baad7d6f9dd40a68a26ed55fe37bbd?size=1024"
        /></ul>
            <ul class="flex w-[260px]">
        <Card 
          href="https://github.com/Butwm"
          title="Butwm"
          role="Developer"
          body=""
          image="https://cdn.discordapp.com/avatars/795996972758204426/1fedd8ab05818df52c73fc621bb8f816?size=1024"
        /> </ul>
            <ul class="w-[260px]">
        <Card 
          href="#"
          title="Matus Kazik"
          role="CEO"
          body="So excited for this!"
          image="https://framerusercontent.com/images/nv4BiIDU0mxJlQD7YTEV67CKv0.jpg?scale-down-to=1024"
        /></ul>
        <ul class="w-[280px]">
        <Card 
          href="#"
          title="Pavel Malaska"
          role="Manager"
          body="Can't wait for the open!"
          image="https://cdn.discordapp.com/avatars/573928034818588703/f6766e597447c7cced6dd95fd0e5d692?size=1024"
        />
        </ul>     
        </li>
      </div>
    </div>
  </template>
  
  <script>
  import Card from '../cardslider/Card.vue';
  
  export default {
    components: {
      Card,
    },
  };
  </script>
  
  <style>
  .container {
    position: relative;
    width: 100%;
    height: 200px;
    overflow: hidden;
  }
  
  .moving-element {
    position: absolute;
    top: 0; 
    left: 0; 
    width: max-content;
    height: 50px;
    background-color: rgb(126, 126, 231);
    animation: moveRightToLeft 25s linear infinite;
    display: flex;
    animation-delay: -0s; /* Delay the start of the animation to allow time for initial scrolling */
  }
  
  @keyframes moveRightToLeft {
    0% {
      transform: translateX(100%); 
    }
    100% {
      transform: translateX(-100%); 
    }
  }
  </style>
  