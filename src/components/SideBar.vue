<template>
    <div class="w-1/3 bg-white h-full p-9 z-50 border-2 border-r-[#E2E2E2]">
        <div class="flex flex-col">
            <h1 class="font-bold text-4xl mb-9">Uni<span class="text-[#F0394F]">verse</span></h1>
            <SidebarItem title="Home" :icon="require('@/assets/img/home.png')" :isActive="$route.path === '/'" @click.native="$router.push({ path: '/' })" />
            <SidebarItem title="Profile" :icon="require('@/assets/img/profile.png')" :isActive="$route.path === '/profile'" @click.native="$router.push({ path: '/profile' })" />
            <SidebarItem title="Explore Communities" :icon="require('@/assets/img/profile.png')" :isActive="$route.path === '/explore-communities'" @click.native="$router.push({ path: '/explore-communities' })"/>
            <SidebarItem title="Settings" :icon="require('@/assets/img/settings.png')" :isActive="$route.path === '/settings'" @click.native="$router.push({ path: '/settings' })"/>
            <hr class="border-t-2 border-gray-200 my-14 w-full">
            <div class="flex flex-row justify-between">
                <h3 class="text-[#535353] text-xl font-bold">My Communities</h3>
                <span class="bg-[#F0394F] py-1 text-white px-4 rounded-full">19</span>
            </div>
            <Community name="Web Development" members="764" :icon="require('@/assets/img/community1.png')"/>
            <Community name="PHP Laravel" members="480" :icon="require('@/assets/img/community1.png')"/>
            <Community name="Python Django" members="540" :icon="require('@/assets/img/community1.png')"/>

            <a href="" class="p-4 rounded-lg border-2 border-[#F0394F] text-center text-[#F0394F] font-semibold">See All</a>
        </div>
    </div>
</template>
  
<script>

import SidebarItem from './SidebarItem.vue';
import Community from './Community.vue';
export default{
    name: "SideBar",
    components: {
        SidebarItem,
        Community
    },
    data() {
        return {
            activeItem: 'Home', 
        }
    },
    methods: {
        setActiveItem(item) {
        this.activeItem = item;
        }
    }
};
</script>