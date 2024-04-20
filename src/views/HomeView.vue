<template>
  <div class="flex flex-col h-screen">
    <Header />
    <div class="flex flex-row flex-grow">
      <SideBar />
      <Post />
      <div class="flex flex-col mt-32">
        <RecentsModal filter="Based on Your Communities"/>
        <RecentsModal filter="People You May Know" :peopleYouMayKnow="peopleYouMayKnow"/>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Post from "@/components/Post.vue";
import SideBar from "@/components/SideBar.vue";
import Header from "@/components/Header.vue";
import RecentsModal from "@/components/RecentsModal.vue";

export default {
  name: "HomeView",
  components: {
    SideBar,
    Header,
    Post,
    RecentsModal,
  },
  data() {
    return {
      filter: "Based on Your Communities",
      peopleYouMayKnow: [
        {
          name: "Miles Morales",
          user: require("@/assets/img/user.png"),
          action: "Follow",
          role: "DevOps Engineer",
        },
        {
          name: "Peter Parker",
          user: require("@/assets/img/user.png"),
          action: "Follow",
          role: "IT Manager",
        },
        {
          name: "GwenStacy",
          user: require("@/assets/img/user.png"),
          action: "Follow",
          role: "State Registered Nurse",
        },
        {
          name: "Miles Morales",
          user: require("@/assets/img/user.png"),
          action: "Follow",
          role: "Penetration Tester",
        },
        
      ]
    };
  },
};
</script>