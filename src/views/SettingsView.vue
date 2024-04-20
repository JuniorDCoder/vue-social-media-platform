<template>
    <div class="flex flex-col h-screen">
      <Header />
      <div class="flex flex-row flex-grow">
        <SideBar />
      </div>
    </div>
</template>
<script>
import SideBar from '@/components/SideBar.vue'
import Header from '@/components/Header.vue'
export default{
    components: {
        SideBar,
        Header
    }
}
</script>