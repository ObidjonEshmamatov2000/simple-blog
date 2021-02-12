<template>
    <div>
        <div class="my-12 text-center px-16">
            <h2 class="text-h3 my-4">About Blog</h2>
            <p class="text-subtitle-1 mb-4">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Expedita soluta voluptates quaerat, minima harum vero! Tenetur, ea quod! Aut quod qui, eveniet voluptatem repudiandae molestias rem quidem aperiam cumque sequi.</p>
        </div>
        
        <v-container>
            <v-row>
                <v-col cols="12" py-8>
                    <div class="posts-div mb-8">
                        <p class="posts mt-3">Create awesome websites using Vue.js</p>
                    </div>
                </v-col>
            </v-row>
            <v-row>
                <v-col cols="12" class="text-center">
                    <a class="my-4" href="https/obidjon-2000.web.app">View Real Demo</a>
                    <v-img class="my-4" src="../assets/6.jpg"></v-img>
                    <p class="text-subheading-1">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nam fugit assumenda quasi molestiae, quia enim quis. Ipsam, nostrum illo itaque consectetur, distinctio in a, doloribus nisi excepturi molestias consequuntur rem.</p>
                </v-col>
            </v-row>
        </v-container>
    </div>
</template>

<script>
export default {
    name: 'Posts',
    components: {
        
    }
}
</script>

<style scoped>
    .posts-div {
        background-color: #5281b9;
        text-align: center;
        padding: 20px;
        color: white;
    }
    .posts {
        font-size: 26px;
    }
</style>