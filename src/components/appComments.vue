<template>
          
        <div class="card mb-10 comment--item">
          <p>
           {{content}}
          </p>
          <div class="action--button--container text-right mt-10">
            <button @click="likeCounter++" class="btn-sm btn-success">Beğendim ({{likeCounter}})</button>
            <button @click="disslikeCounter++" class="btn-sm btn-danger">Beğenmedim ({{disslikeCounter}})</button>
          </div>
        </div>
        

</template>

<script>
export default {
  props: ['content'],
  data(){
    return{
      likeCounter:0,
      disslikeCounter:0
    }
  }
}
</script>