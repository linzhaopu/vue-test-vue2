<template>
  <h2 class="red" @tap="tap1">test...{{msg}}</h2>
</template>

<script>
export default {
    name:'test',
    props: {
        msg: {
            type: String,
            default: "test msg"
        }
    },
    methods: {
        tap1: function(){
            console.log(1);
            this.$emit('tap1',this.msg);
        }
    }

}
</script>

<style>
.red{
    color:red;
}
</style>