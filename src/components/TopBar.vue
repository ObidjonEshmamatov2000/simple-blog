<template>
    <div class="mb-16">
        <v-app-bar class="px-sm-16" color="white" fixed>
            <v-toolbar-title class="grey--text text--darken-2 pl-sm-10"><v-list-item class="white blue-grey--text text--lighten-1" to="/">Blog</v-list-item></v-toolbar-title>
            <v-spacer></v-spacer>

            <span class="hidden-sm-and-up">
                <v-btn @click="drawer = !drawer" text>
                    <v-icon color="black">fa-bars</v-icon>
                </v-btn>
            </span>

            <v-toolbar-items class="hidden-xs-only pr-sm-8">
                <v-btn class="blue-grey--text text--lighten-1"  to="/" text>
                    Home
                </v-btn>
                <v-btn class="blue-grey--text text--lighten-1" to="/posts" text>
                    Posts
                </v-btn>
                <v-btn class="blue-grey--text text--lighten-1" to="/about" text>
                    About
                </v-btn>
            </v-toolbar-items>
        </v-app-bar>

        <v-navigation-drawer
            v-model="drawer"
            absolute
            temporary
            right
            class="transition pt-8"
        >
            <v-list>
                <v-list-item to="/" link>
                    <v-btn text block>
                        Home
                    </v-btn>
                </v-list-item>
                <v-list-item to="posts" link>
                    <v-btn text block>
                        Posts
                    </v-btn>
                </v-list-item>
                <v-list-item to="about" link>
                    <v-btn text block>
                        About
                    </v-btn>
                </v-list-item>
                
            </v-list>
        </v-navigation-drawer>
    </div>
</template>

<script>
export default {
    data() {
        return {
            drawer: false
        }
    }
}
</script>

<style scoped>
    .transition {
        transition: .5s ease all;
    }
</style>