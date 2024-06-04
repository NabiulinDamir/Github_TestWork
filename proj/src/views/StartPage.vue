<template>
    <div class="WebName">
        ВИКЕНТЕВА.РУ
    </div>
    <div class="choice">
        <router-link class="choice__link">ПНИПУ</router-link>
        <router-link class="choice__link">ПГУ</router-link>
        <!-- <div class="Choice__Button">ПНИПУ</div>
        <div class="Choice__Button">ПГУ</div> -->
    </div>
</template>

<script setup>
import {ref} from 'vue';
import ChoiseButton from '/src/components/StartPageComponents/ChoiseButton.vue'

const link_1 = ref({name: 'ПНИПУ', href: '/typography'})
    

</script>

<style lang="scss" scoped>
.choice{
    // background-color: aqua;
    display: flex;
    justify-content: center;
    

    &__link {
        width: 150px;
        height: 50px;
        margin-left: 40px;
        margin-right: 40px;
        display: flex;
        border-radius: 12px;
        padding: 10px;
        border: 2px solid #6979f8;
        color: #6979f8;
        transition:  0.2s;
        font-weight: bold;
        // margin-bottom: 10px;
        place-content: center;
        align-items: center;
        font-size: 1.5em;
        text-decoration: none;
        &:hover{
            border-color: #5b68c8;
            color: #5b68c8;
        }
    }
}
</style>