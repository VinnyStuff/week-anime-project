<template>
    <div class="Navbar">
        <div id="navbar-container">
            <h3 id="season">{{currentSeason}} Winter</h3> <!-- winter is a example to make the css-->
            <div id="week">
                <button @click="monday">Monday</button>
                <button>Tuesday</button>
                <button>Wednesday</button>
                <button>Thursday</button>
                <button>Friday</button>
                <button>Saturday</button>
                <button>Sunday</button>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    props: ["currentSeason"],
    methods:{
        monday(){
            console.log("monday");
        }
    }
}
</script>

<style scoped>
    #navbar-container{
        background-color: black;
        color: white;
    }
    #week > button{
        margin: 20px;
        background-color: transparent;
        color: white;
        padding: 20px;
    }
</style>