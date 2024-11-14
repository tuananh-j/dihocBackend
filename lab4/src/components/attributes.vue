<template>
    <div class="container">
        <h5 v-bind:class="classContent" v-html="content">

        </h5>
    </div>
    <div>
        <button class ="btn btn-primary" v-on:click ="success">
            click me
        </button>
    </div>
</template>
<script>
    export default{
        data(){
            return{
                content : "hi i'm tuan anh",
                classContent : 'text-info'
            }
            
        },
        methods:{
            success: function(){
                Swal.fire({
                title: "Good job!",
                text: "You clicked the button!",
                icon: "success"
                });
            }
        }

    }
</script>
<style>

</style>