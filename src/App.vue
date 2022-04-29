<template>
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Comment Like/Dislike App</title>
  </head>
  <body>
    <header>Comment Like/Dislike App</header>
    <div class="container">
      <div  class="comment--like--dislike--app">
            <ul v-for="comment in commentList" :key="comment.id">
        <appComments :content="comment.content"   />
        </ul>
   

  
      </div>
    </div>
  </body>
</html>

</template>


<script>
import appComments from "@/components/appComments"
export default {
  
  data(){
    return {
      commentList: [{id: 1, content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint deserunt, tempore accusamus iusto nobis dolore ratione itaqueperferendis delectus? Nostrum corporis, quod voluptates quis consequuntur eveniet beatae dolor aperiam ad.'},
      {id: 2, content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint deserunt, tempore accusamus iusto nobis dolore ratione itaqueperferendis delectus? Nostrum corporis, quod voluptates quis consequuntur eveniet beatae dolor aperiam ad.'},
      {id: 3, content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint deserunt, tempore accusamus iusto nobis dolore ratione itaqueperferendis delectus? Nostrum corporis, quod voluptates quis consequuntur eveniet beatae dolor aperiam ad.'},
      {id: 4, content: 'Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sint deserunt, tempore accusamus iusto nobis dolore ratione itaqueperferendis delectus? Nostrum corporis, quod voluptates quis consequuntur eveniet beatae dolor aperiam ad.'}],
      
    }
  },
  components : {
    appComments
  }
}
</script>

<style >
@import 'assets/style.css';
</style>
