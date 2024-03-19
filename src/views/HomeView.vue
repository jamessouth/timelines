<script setup>
import { ref } from 'vue'
    import GameArea from '../components/GameArea.vue'
    import ListButtons from '../components/ListButtons.vue'

    let ind = ref(0);

    let msgs = ref([{msg:"aaa", new:false}, {msg:"bbb", new:false}, {msg:"ccc", new:false}, {msg:"ddd", new:false}, {msg:"eee", new:false}, {msg:"fff", new:false}, {msg:"ggg", new:false}, {msg:"hhh", new:false}, {msg:"iii", new:false}]);

    function moveDown(){
        let k = {msg:"xxzx", new:true};
        ind.value++;
        // let k = msgs.reverse();
        console.log(ind.value);
        msgs.value = msgs.value
        .filter(x => !x.new)
        .toSpliced(ind.value, 0, k);
        console.log(msgs.value);


        
    }
</script>

<template>
  <main>
    <GameArea :msgs="msgs"/>
  </main>
  <section>
    <ListButtons :md="moveDown"/>
    
  </section>
</template>
