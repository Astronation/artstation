<template>
  <div class="w-full md:w-6/12 lg:w-3/12 lg:mb-0 mb-12 px-4">
    <a 
      :href="link"
      target="_blank" 
    >
      <div class="px-6">
        <img
          :src="profilePic"
          class="shadow-lg rounded-lg mx-auto max-w-120-px"
        />
        <div class="pt-6 text-center">
          <h5 class="text-xl font-bold">{{nickname}}</h5>
          <p
            class="mt-1 text-sm text-blueGray-400 uppercase font-semibold"
          >
            {{role}}
          </p>
        </div>
      </div>
    </a>
  </div>
</template>

<script>
export default {
 props: ['profile-pic', 'nickname', 'role', 'link']
}
</script>