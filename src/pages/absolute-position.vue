<template>
  <q-page class="flex flex-center">
    <div class="parent">
      <div class="child">1</div>
      <div class="child">2</div>
      <div class="child absolute">3</div>
    </div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>

<style scoped lang="scss">
.parent {
  height: 500px;
  border: 5px dotted lightgray;
  padding: 10px;
  position: relative; /*parent가 child의 기준점이 됨*/
}

.child {
  width: 150px;
  height: 100px;
  border: 3px dotted crimson;
  border-radius: 12px;
  background-color: lightyellow;
}

.absolute {
  position: absolute;
  bottom: 50px;
}
</style>
