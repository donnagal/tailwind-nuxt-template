<template>
  <div class="container mx-auto pt-32">
    <article>
      <h2>{{post.title}}</h2>
      <p>{{post.content}}</p>
    </article>
    <div>
      <h3>Posts you might enjoy</h3>
      <ul>
        <li v-for="related in relatedPosts">
           <nuxt-link class="underline" :to="{name: 'posts-id', params: {id: related.id}}">
           {{related.title }}
           </nuxt-link>
          <!-- <nuxt-link  class="underline" :to="`/posts/${related.id}`">{{related.title }}</nuxt-link> -->
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        id: this.$route.params.id,
        posts: [
          {
            id: 'blog',
            title: 'Edition 01',
            content: 'If someone placed balut on your plate, you might think they were serving you a hardboiled egg. That is, until you cracked it open and a fully intact duck embryo spilled out. Balut, considered a delicacy in many Asian countries, is produced when fertilized duck eggs are placed in warm sunlight. After about eight days, the eggs are held up to the light and checked to ensure that the budding embryo is ready. Then, the eggs are cooked and served with a dash of salt and a few squirts of lemon juice.'
          },
          {
            id: 'blog-2',
            title: 'Edition 02',
            content: 'I\'ve stalked the forum for a while, reading everything closely, but today I decided that it was time to register as a user. So I did, this morning! But now, when I came back to the forum, I cannot seem to find the damn sign in button? WHERE IS IT???!??'
          },
          {
            id: 'blog-3',
            title: 'Edition 03',
            content: 'Please help me. I dont know what is the best way to fix my problem. I cant reproduce and I cant tell more info. Can someone help me asap??? I am in a hurry!!!'
          }
        ]
      }
    },
    computed: {
      post () {
        return this.posts.find(post => post.id === this.id)
      },
      relatedPosts(){
        return this.posts.filter( post => post.id !== this.id)
      }
    }
  }
</script>

<style scoped>
</style>