<template>
  <div class="b">
      
<h1>Rikshaw</h1>
      </div>
      

</template>

<script>
export default {
    name: 'Rikshaw',

    activated(){
            console.log('activated')
    },
    deactivated(){
            console.log('disactivated')
    },
    destroyed(){
            console.log('destroyed')
    }
}
</script>

<style scoped>

div.b{
    border: 1px dotted blue;
}
</style>