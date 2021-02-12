<template>
    <v-container>
        <v-row>
            <v-col cols="12" class="text-center d-flex flex-column align-center justify-center pt-16 mt-12">
                <h2 class="text-h4 mb-5">Comments:</h2>
                <v-container>
                    <v-row>
                        <v-col offset="2" cols="8" class="white mb-6 py-6 px-10" v-for="(comment, i) in comments" :key="i">
                            <div class="commenter mb-3">{{ comment.name}}</div>
                            <div class="comment">{{ comment.text }}</div>
                        </v-col>
                    </v-row>
                </v-container>
            </v-col>

            <v-col cols="12" class="text-center d-flex flex-column align-center justify-center pt-16 mt-12">
                <h2 class="text-h4 mb-5">New Comment:</h2>
                <v-container>
                    <v-row>
                        <v-col offset="3" cols="6" class="mb-6 py-6">
                            <v-text-field
                                solo
                                label="Name"
                                placeholder="Your name"
                                outlined
                                dense
                                class="py-6 white--text"
                                rounded
                                elevation="2"
                                v-model="newCommenter"
                            ></v-text-field>
                            <v-textarea
                                solo
                                name="input-7-4"
                                label="Your comment..."
                                rounded
                                v-model="newComment"
                                class="align-left"
                            ></v-textarea>
                                <v-btn
                                    rounded
                                    color="primary"
                                    dark
                                    class="px-10 py-5"
                                    large
                                    @click.prevent="submit"
                                >
                                    Submit
                                </v-btn>
                        </v-col>
                    </v-row>
                </v-container>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    data() {
        return {
            comments: [
                { name: 'Alex', text: 'Lookup 👀 😛'},
                { name: 'Gesa', text: 'Sweeeeeet!'},
            ],
            newCommenter: '',
            newComment: ''
        }
    },
    methods: {
        submit: function() {
            this.comments.push({
                name: this.newCommenter,
                text: this.newComment
            })

            this.newComment = '';
            this.newCommenter = '';
        }
    }

}
</script>

<style scoped>
    .commenter {
        font-size: 24px;
        color: #5c4de7;
        letter-spacing: 1.2;
    }
    .comment {
        font-size: 18px;
        color: #101010;
    }
</style>