<template>
  <div class="home">
    <h1>Home</h1>
    <PostList :posts="posts"/>
  </div>
</template>
<script>
import { ref } from '@vue/reactivity'
import PostList from '../components/PostList.vue';
export default {
    name: "HomeView",
    components:{PostList},
    setup() {
        const posts = ref([
            {
                title: "welcome o the blog",
                body: " Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, voluptas optio sit cupiditate blanditiis dicta, sunt quisquam eaque quo, in eligendi repudiandae! Quia accusamus sunt nobis voluptatum porro at corrupti!Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, voluptas optio sit cupiditate blanditiis dicta, sunt quisquam eaque quo, in eligendi repudiandae! Quia accusamus sunt nobis voluptatum porro at corrupti!Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, voluptas optio sit cupiditate blanditiis dicta, sunt quisquam eaque quo, in eligendi repudiandae! Quia accusamus sunt nobis voluptatum porro at corrupti!Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, voluptas optio sit cupiditate blanditiis dicta, sunt quisquam eaque quo, in eligendi repudiandae! Quia accusamus sunt nobis voluptatum porro at corrupti!Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, voluptas optio sit cupiditate blanditiis dicta, sunt quisquam eaque quo, in eligendi repudiandae! Quia accusamus sunt nobis voluptatum porro at corrupti!Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, voluptas optio sit cupiditate blanditiis dicta, sunt quisquam eaque quo, in eligendi repudiandae! Quia accusamus sunt nobis voluptatum porro at corrupti!",
                id: 1
            },
            {
                title: "top 5 CSS tip",
                body: "loremipsum",
                id: 2
            }
        ]);
        return { posts };
    },
     
}
</script>
