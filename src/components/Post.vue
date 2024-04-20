<template>
    <div class="mt-32 mb-4 mx-9 bg-white w-2/3 flex-grow rounded-lg">
        <div class="flex flex-col p-7">
          <div class="flex space-x-2 flex-row">
            <img :src="require('@/assets/img/user.png')" class="w-16 h-16" alt="">
            <div class="flex flex-row space-x-4 mt-2">
              <h3 class="font-semibold">You</h3>
              <span class="font-bold"> > </span>
              <h3 class="font-semibold text-[#F0394F]">PHP Laravel</h3>
            </div>
          </div>
          <div class="mt-2 leading-7 font-semibold">
            <p>Top GitHub repositories to learn modern React development. Open source is great for 
              many things. One of them is learning new skills. In this article, we'll look at some of the best 
              Open Source React projects on GitHub that you can use to quickly boost your hands-on React 
              learning and coding experience.
            </p>
            <img :src="require('@/assets/img/post1.png')" class="py-3" alt="">
            
          </div>
          <p class="text-xl font-semibold"><i class="fas fa-heart text-[#F0394F]"></i> Joe, Shaan & 3 others like this</p>
          <div class="mt-3">
            <h3 class="text-[#F0394F] font-semibold text-xl mb-2">Comments</h3>
          
            <div class="relative">
              <div class="flex flex-row space-x-2 bg-[#F5F5F5] p-2 rounded-lg">
                <img :src="require('@/assets/img/user.png')" class="w-12 h-12" alt="">
                <div class="flex flex-col space-y-1">
                  <h3 class="font-bold text-sm text-[#F0394F]">Foryoung Junior</h3>
                  <p>Great article, thanks for sharing!</p>
                  <div class="flex flex-row space-x-3 text-gray-400 text-sm muted">
                    <p>32 likes</p>
                    <a href="">like</a>
                    <a href="">Reply</a>
                  </div>
                </div>
              </div>
              <div class="absolute left-6 top-20 bottom-9 border-l border-dotted border-gray-400"></div>
              <div class="flex mt-2 w-1/3 ml-24 flex-row space-x-2 bg-[#F5F5F5] p-2 rounded-lg">
                <img :src="require('@/assets/img/user.png')" class="w-12 h-12" alt="">
                <div class="flex flex-col space-y-1">
                  <h3 class="font-bold text-sm text-[#F0394F]">Shaan Alam</h3>
                  <p>Great article, thanks for sharing!</p>
                  <div class="flex flex-row space-x-3 text-gray-400 text-sm muted">
                    <a href="">like</a>
                    <a href="">Reply</a>
                  </div>
                </div>
              </div>
              <div class="absolute left-5 right-0 top-36 w-1/12 border-t border-dotted border-gray-400"></div>
            </div>
          </div>
          
        </div>
    </div>
</template>

<script>

</script>