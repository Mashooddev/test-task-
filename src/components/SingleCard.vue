<template>
    <div>
      <figure class="w-full h-[250px] my-2">
        <img :src="image" alt="image" class="rounded-md h-full w-full">
      </figure>
      <div class='flex items-start gap-2'>
        <img :src="profileImage" alt="profileimage" class='h-10 w-10 object-cover rounded-full'/>
        <div>
          <h5 class='font-semibold text-lg'>{{ name }}</h5>
          <p class="font-normal text-base">{{ title }}</p>
          <p class="font-normal text-sm">{{ views }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      image: {
        type: String,
        default: ""
      },
      profileImage: {
        type: String,
        default: ""
      },
      name: {
        type: String,
        default: ""
      },
      title: {
        type: String,
        default: ""
      },
      views: {
        type: Number,
        default: 0
      }
    }
  }
  </script>
  