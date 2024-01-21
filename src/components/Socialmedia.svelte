<script lang="ts">
  export let socialUrl = "";
  export let socialName = "";
</script>
<div class="group bg-zinc-700 text-center 
  w-80 h-16 py-2 mx-12 rounded-xl 
  flex justify-center items-center 
  hover:bg-lime-500">
  <a
    href={socialUrl}
    target="_blank"
    class="text-gray-50 font-bold group-hover:text-black"
  >{socialName}</a>
</div>
