<template>
 <div>

    <button :class="button" @click="handleclick"></button>
 </div>
</template>

<script>
export default {

    name: "my button",
    props: {
        button: {
            type: String,
            required: true
        },
    
    buttonText: {
        type: String,
        default: 'Click Me'
    }, 

    }, 
    methods: {
        handleclick() {
            this.$emit('click');
        }
    }
};

</script>

