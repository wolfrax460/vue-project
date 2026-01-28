    
    
<template>
  <div>
    <button @click="flipCoin">Flip Coin</button>
    <p v-if="result">{{ result }}</p>
    
  </div>
</template>

<script>
export default {
  data() {
    return {
      result: null
    };
  },
  methods: {
    
    flipCoin() {
      this.result = Math.random() < 0.5 ?'Heads' : 'Tails';
    }
  }

};
</script>

<style>

</style>