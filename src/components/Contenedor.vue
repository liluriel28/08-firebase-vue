<template>
    <div class="row">
        <div class="col s12 m7">
            <card-project/>
            <card-project/>
        </div>
    </div>
    
</template>
<script>
import CardProject from './CardProject.vue';

export default {
    data:()=> ({
        projects:null, 
    }),
    
    components: {
         CardProject 
    },
    mounted(){
        this.getProjects();
    },
    methods:{
        async getProjects(){
            const res= await fetch("https://miko-quir-4b2a9-default-rtdb.firebaseio.com/projects/project.json");
            const data = await res.json();

            console.log(data);
        },
    },
};
</script>
