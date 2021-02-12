<template>
    <div>
        <div class="my-12"></div>
        <div class="posts-div mb-8">
            <p class="posts mt-3">My Posts:</p>
        </div>
        <v-container>
            <v-row class="d-flex justify-space-between">
                <v-col cols="12" sm="6" md="4" class="d-flex flex-column align-center justify-center">
                    <v-img src="../assets/1.jpg"></v-img>
                    <h2 class="text-h5 my-3">Quis Nostrud!</h2>
                    <p class="text-subtitle-1">Lorem ipsum dolor sit amet.</p>
                </v-col>
                <v-col cols="12" sm="6" md="4" class="d-flex flex-column align-center justify-center">
                    <v-img width="100%" src="../assets/2.jpg"></v-img>
                    <h2 class="text-h5 my-3">Nemo</h2>
                    <p class="text-subtitle-1">Lorem ipsum dolor sit amet.</p>
                </v-col>
                <v-col cols="12" sm="6" md="4" class="d-flex flex-column align-center justify-center">
                    <v-img width="100%" src="../assets/3.jpg"></v-img>
                    <h2 class="text-h5 my-3">Set Uit</h2>
                    <p class="text-subtitle-1">Lorem ipsum dolor sit amet.</p>
                </v-col>
            </v-row>
        </v-container>
        <Main />
    </div>
</template>

<script>
import Main from '../components/Main'
export default {
    name: 'Posts',
    components: {
        Main
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