<template>
<div class="backdrop"> 
  <div class="modal">
    <p>{{header}}</p>
     <h1> content </h1>
     <p> {{text}} </p>
  </div>
  </div>
</template>

<script>
export default {
  props: ['header', 'text']
}
</script>


<style scoped>
 .modal {
    width: 400px;
    padding: 20px;
    margin: 200px auto;
    background: white;
    border-radius: 10px;
  }
  .backdrop {
    top: 0;
    position: fixed;
    background: rgba(0,0,0,0.5);
    width: 100%;
    height: 100%;
  }
  .modal h1 {
    color: #996;
    border: none;
    padding: 0;
  }
  .modal p {
    font-style: normal;
  }
  /* sale styles */
  .modal.sale {
    background: crimson;
    color: white;
  }
  .modal.sale h1 {
    color: white;
  }
</style>
