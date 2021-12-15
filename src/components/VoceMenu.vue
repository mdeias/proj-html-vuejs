<template>
  <li>
      {{voce}} <i class="fas fa-chevron-down"></i>
  </li>
</template>

<script>
export default {
    name: 'VoceMenu',

    props:{
        voce: String
    }
}

</script>

<style>
.fa-chevron-down{
    font-size: 8px;  
}
</style>