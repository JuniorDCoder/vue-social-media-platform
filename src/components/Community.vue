<template>
    <a href="" class="flex flex-row my-4 space-x-3">
        <img :src="icon" class="w-[78px]" alt="">
        <div class="flex flex-col mt-4 text-[#535353]">
            <h1 class="font-semibold">{{name}}</h1>
            <p class="text-sm">{{ members }} members</p>
        </div>
    </a>
</template>

<script>
export default{
    props: {
        name: {
            type: String,
            default: "Community"
        },
        members: Number,
        icon: String
    },
}
</script>