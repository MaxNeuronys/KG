<template>
    <div class="postits">
        <this-postit v-for="postit in postits"
        :key="postit.id"
        :title="postit.title"
        :description="postit.description"
         />
    </div>
    
</template>
<script>
import ThisPostit from './thisPostit.vue'
export default {
    name:"postits",
    components:{ThisPostit},
    data(){
        return{
            postits : [{
                id: "1",
                title : "My first post it title",
                description : "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Duis imperdiet nec dolor in faucibus. Nulla convallis bibendum congue. Quisque in ipsum suscipit, mattis dolor nec, mollis est. Integer vel lobortis velit. Nullam commodo magna dolor, eu interdum odio cursus eu. Suspendisse faucibus ac ligula vitae tincidunt. Maecen"},
                {
                id: "2",
                title : "My 2nd post it title",
                description : "Elementum massa interdum nec. Praesent at dui quis orci lobortis maximus non ac elit. Morbi iaculis lacus nec odio blandit finibus. Proin sit amet felis arcu. In eleifend semper pellentesque. Nam pellentesque ullamcorper lacinia. Vestibulum tincidunt efficitur justo, a interdum lectus dictum nec. Vivamus id mollis enim, a tinci."},

                {
                id: "3",
                title : "My 3rd post it title",
                description : "Bitasse platea dictumst. In tincidunt nibh eros, quis commodo odio tincidunt vitae. Phasellus dictum erat quis elit ultrices tincidunt. Vivamus efficitur ultricies convallis. Suspendisse sed dolor at ipsum condimentum cursus. Proin feugiat ante sed vestibulum scelerisque. Proin et sem metus. Nullam aliq."
            }],
            commandes: [],
            affichage: "display-4",
            unique: false,
        }
    }, 
}
</script>
<style scoped>
.postits{

}
</style>