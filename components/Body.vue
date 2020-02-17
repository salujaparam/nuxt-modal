
<template>
    <div class="body">
        <!-- <hr /> -->
        <form class="desc">
            <textarea id="w3mission" rows="6" cols="52" placeholder="Go Ahead write about yourself..."/>
        </form>
        <!-- <hr /> -->
        <div class="buttons">
            <button class="close" @click="$emit('close-modal')">Close</button>
            <button class="save" @click="$emit('close-modal')">Save Changes</button>
        </div>
    </div>
</template>
    
<style scoped>
    .body {        
        padding-top: 20px;
    }
    .desc {
        /* padding: 10px; */
        width: 100%;
        height: 100%;
        border-top: 1px solid #DCDCDC;
        border-bottom: 1px solid #DCDCDC; 
    }
    textarea {
        resize: none;
        border: none;
        /* background-color: #DCDCDC; */
    }
    textarea::placeholder{
        padding-top: 2rem;
        text-align: center;
    }
    .buttons {
        padding: 1rem 0 0 13rem;
    }
    .close {
        background-color: #A9A9A9;
        color: white;
        width: 4rem;
        height: 2.5rem;
        border: none;
        border-radius: 10px;
        cursor: pointer;
    }
    .save {
        background-color: #1E90FF;
        color: white;
        width: 7rem;
        height: 2.5rem;
        border: none;
        border-radius: 10px;
        cursor: pointer;
    }
</style>