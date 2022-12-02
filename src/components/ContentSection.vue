<template>  
    <div class="content_section">
        <div class="container">
            <div class="content_box">
               <div>| Contenuto |</div>
            </div>
        </div>
    </div>

</template>

<script>
    export default{
        data(){
            return{
                
            }
        }
    }
</script>


<style scoped>
    .content_section{
        min-height: 100px;
        background-color: #1C1C1C;
    }

    .content_box{
        height: 100px;
        color: white;
        display: flex;
        align-items: center;
    }
</style>