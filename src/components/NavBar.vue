<template>
    <nav>
        <v-toolbar dark app>
            <v-toolbar-side-icon class="grey--text" @click="drawer = !drawer"></v-toolbar-side-icon>
            <v-toolbar-title class="text-uppercase grey--text">
                <span class="font-weight-light">todo</span>
                <span>eyy</span>
            </v-toolbar-title>
            <v-spacer></v-spacer>
            <v-btn flat color="grey">
                <v-icon left>favorite</v-icon>
                <span>gato</span>
            </v-btn>
        </v-toolbar>
        <v-navigation-drawer app v-model="drawer"  class="primary">
            <v-list>
                <v-list-tile v-for="link in links" :key="link.text" router :to="link.route">
                    <v-list-tile-action>
                        <v-icon class="white--text">{{link.icon}}</v-icon>
                    </v-list-tile-action>
                    <v-list-tile-content>
                        <v-list-title-content class="white--text">
                            {{link.text}}
                        </v-list-title-content>
                    </v-list-tile-content>
                </v-list-tile>
            </v-list>
        </v-navigation-drawer>
    </nav>
</template>
<script>
/* eslint-disable */
export default {
    data(){
        return{
            drawer:false,
            links:[
                {icon: 'dashboard',text:'Dashboard', route:'/'},
                {icon: 'folder', text:'Mi proyecto', route:'/projects'},
                {icon: 'person',text:'Team', route:'/team'}
                ]
        }
    }
}
</script>
