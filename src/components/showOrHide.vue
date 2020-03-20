<template>
    
    <div class="showHide">
        
    <h2>{{headline}}</h2>
    <div class="line"></div>


    </div>

</template>
<script>
export default {
    data: () => ({
       headline:"Show or Hide"

    })
    
}
</script>

<style scope>
.showHide{
    background-color:rgb(138, 207, 138);
}
h2{
    padding:0.5em;
}
.line{
    border-top:3px solid rgb(131, 161, 168);
    margin:0 3em 0;
    border-radius:2px;
    padding:1em;
}

</style>