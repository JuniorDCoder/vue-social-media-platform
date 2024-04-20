<template>
    <div class="bg-white flex flex-col rounded-lg mb-4 w-[300px] mr-12 h-2/3 p-4">
        <h3 class="font-semibold text-[#F0394F] mb-3">{{filter}}</h3>
        <div v-if="peopleYouMayKnow.length != 0">
            <RecentItem v-for="person in peopleYouMayKnow" :key="person.name" :user="person.user" :name="person.name" :members="person.role" :action="person.action"/>
        </div>
        <div v-else>
            
            <RecentItem :user="require('@/assets/img/user.png')" name="Python Django" members="540" action="Join"/>
            <RecentItem :user="require('@/assets/img/user.png')" name="PHP Laravel" members="380" action="Join"/> 
            <RecentItem :user="require('@/assets/img/user.png')" name="DevSecOps" members="240" action="Join"/>
            <RecentItem :user="require('@/assets/img/user.png')" name="DevSecOps" members="240" action="Join"/>
            <RecentItem :user="require('@/assets/img/user.png')" name="DevSecOps" members="240" action="Join"/>
        </div>
    </div>
    
</template>

<script>
import RecentItem from './RecentItem.vue';
export default{
    
    components: {
        RecentItem,
    },
    props: {
        filter: String,
        peopleYouMayKnow: {
            type: Array,
            default: () => [],
        }
    },


}
</script>