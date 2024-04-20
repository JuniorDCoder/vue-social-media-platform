<template>
    <div class="fixed right-0 w-full -z-0 bg-white h-24">
        <div class="flex flex-row justify-end p-4 space-x-4">
            <a href=""class="bg-[#E7E7E7] w-16 h-16 rounded-full flex items-center justify-center">
                <i class="fas fa-envelope fa-lg"></i>
            </a>
            <a href="" class="bg-[#E7E7E7] w-16 h-16 rounded-full flex items-center justify-center">
                <i class="fas fa-bell fa-lg"></i>
            </a>
            <router-link to="/profile" class="flex flex-row items-center space-x-2">
                <img :src="require('@/assets/img/user.png')" class="w-16 h-16" alt="">
                <h3 class="font-semibold truncate">Foryoung Junior</h3>
            </router-link>
            
        </div>
    </div>
</template>
  
<script>
  
</script>