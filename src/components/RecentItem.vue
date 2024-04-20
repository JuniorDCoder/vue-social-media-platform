<template>
    <div class="flex flex-row items-center space-x-4 px-2 my-2">
        <img :src="user" class="w-12 h-12" alt="">
        <div class="flex flex-col pr-12">
          <p class="font-semibold text-[#313131]">{{ name }}</p>
          <p class="text-gray-400 text-xs">{{ members }} members</p>
        </div>
        <div class="flex flex-col">
          <img :src="require('@/assets/img/join.png')" class="w-4 h-4" alt="">
          <p class="text-gray-400">{{ action }}</p>
        </div>
      </div>
</template>

<script>
export default{
    props: {
        name: String,
        members: String,
        user: String,
        action: String
    }
}
</script>