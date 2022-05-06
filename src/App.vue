<template>
    <div class="container">
        <div class="field has-addons">
            <div class="control">
                <input class="input" v-model="message">
            </div>
            <div class="control">
                <button class="button is-primary">Add Item</button>
            </div>
        </div>
        <div class="content">
            <ul>
                <li v-for="(item,index) in items" v-bind:key="index">{{item}}</li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            message: 'Hello Vue!',
            items: ['piim', 'sai', 'leib']
        }
    }
}
</script>

<style>

</style>