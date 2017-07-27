<template>
  <div class="hello">
    <div class="container-fluid">
    <div class="page_bground">
      <div class="bg_foto">
        <div class="bg_darker">        
        {{msg}}
        </div>
      </div>
    </div>
  </div>
</div>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Shalom, I am Hello component'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">

  .container-fluid {
    
    padding:0;
  }
  /* Style for "Rectangle 1 copy" */
  .page_bground {     
    background-color: black;
    height:100%;
    /* Style for "Layer 14"  or add picture*/
    .bg_foto {  
      //position: relative;
      background: url('../assets/500021401.jpg')100% no-repeat;
      background-size: cover;
      height: 100%; 
      /* Style for "Rectangle 1" or make picture darker*/
      .bg_darker{         
        background: rgba(90, 90, 90, 0.4);
        height: 100%;       
      }
    }
  } 

</style>
