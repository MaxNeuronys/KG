<template>
    <div>
        <div class="card card-body">
            <h5 class="card-title">{{ title }}</h5>
            <p>{{ description.slice(0, 179) }} ...</p>
            <button @click="open" type="button" class="btn btn-dark"> > </button>
        </div>

        <div v-if="unique" class="big card-body">
            <button @click="close" type="button" class="btn btn-dark"> X </button>
            <h5 class="card-title">{{ title }}</h5>
            <p>{{ description }} ...</p>

        </div>
    </div>
</template>
<script>
export default {
    name:"thisPostit",
    data(){
        return{
            unique: false
        }
    }, 
    props:{
        key: String,
        title: String,
        description: String,
    },
    methods:{
        open(){
            this.unique = true
        },
        close(){
            this.unique = false
        }
    }
}
</script>
<style scoped>
.card{
    width: 300px;
    height: 300px;

}

</style>