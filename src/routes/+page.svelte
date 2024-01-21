<script lang="ts">
  import Socialmedia from '$components/Socialmedia.svelte'
  let src = '/avatar-jessica.jpeg';
  let socialmedia = {
    github: {
      name: "Github",
      url: "https://github.com/yeeloman"
    },
    linkedin: {
      name: "Linkedin",
      url: "https://github.com/yeeloman"
    },
    instagram: {
      name: "Instagram",
      url: "https://github.com/yeeloman"
    },
    facebook: {
      name: "Facebook",
      url: "https://github.com/yeeloman"
    }
  };
</script>
<div class="w-auto h-auto bg-zinc-800 rounded-xl flex justify-center items-center flex-col">
  <img
    {src}
    alt="profile picture"
    class="rounded-full w-20 h-20 my-4 mt-10"
  >
  <h1
    class="font-bold text-2xl text-white"
  >Jessica Randle</h1>
  <p class="text-lime-500 font-semibold text-xs py-1">London, United Kingdom</p>
  <p class="text-white py-5 text-sm">"Front end developerand avid reader."</p>
  <div class="space-y-2">
    {#each Object.values(socialmedia) as {name, url}}
      <Socialmedia 
      socialUrl={ url }
      socialName={ name }
    />  
    {/each}
    <div class="h-10"></div>
  </div>
</div>
