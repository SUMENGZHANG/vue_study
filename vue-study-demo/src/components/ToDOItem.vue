


<template>

    <div>
        <input type="checkbox" id="todo-item" v-bind:checked="isDone" />
        <label for="todo-item">{{ label }}</label>
    </div>

</template>

<script>
export default {

    props: {
        label: { requeired: true, type: String },
        done: { default: false, type: Boolean },
        id:{required:true,type:String}
    },
    data() {
        return {
            isDone: this.done,
        }
    },


}
</script>