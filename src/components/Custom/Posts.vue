<template>
  <div class="posts">
    <div>
        <b-card title="New Post">
            <b-form-textarea
                id="textarea"
                v-model="post"
                placeholder="Enter something..."
                rows="3"
                max-rows="6"
                v-on:Keyup.enter="addPost()"
                ></b-form-textarea>
                <pre class="mt-3 mb-0"></pre>
                <b-button pill variant="primary" @click="addPost()">Add New Post</b-button>
                <b-button pill variant="primary" class="">Button</b-button>
        </b-card>
        </div>                        
        <div v-for="(post) in posts" :key="post">
            <b-card bg-variant="Primary" text-variant="black" title="Card Title">
               <b-card-text>
                 {{post}}
               </b-card-text>
               <b-button href="#" variant="primary">Go somewhere</b-button>
             </b-card>
        </div>
  </div>    
</template>

<script>
// @ is an alias to /src


export default {
  name: 'posts',
  props: ['Title'],
  components: {

  },
  data(){
    return{
      post: '',
      posts: [],

    }
  },
  methods: {
    addPost(){
      console.log("entrou");
      this.posts.push(this.post);
      this.post = '';
       console.log(this.post);
    }
  }
}
</script>
