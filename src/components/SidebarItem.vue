<template>
    <div>
        <router-link :to="{ name: title }" class="mt-5 flex flex-row w-full py-3 px-4 space-x-3 rounded-lg cursor-pointer hover:bg-[#F1F1F1]"
            :class="{'bg-[#F1F1F1]': isActive}">
            <img :src="icon" alt="icon" />
            <h3 class="text-xl">{{title}}</h3>
        </router-link>
    </div>
</template>

<script>
export default{
    props: {
        title: String,
        icon: String,
        isActive: Boolean,
    },
}
</script>