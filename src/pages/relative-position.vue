<template>
  <q-page class="flex flex-center">
    <div class="grand-parent">
      <div class="parent">
        <div class="child">1</div>
        <div class="child relative">2</div>
        <div class="child">3</div>
      </div>
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
.grand-parent {
  height: 500px;
  border: 5px dotted lightsalmon;
  padding: 50px;
}

.parent {
  height: 500px;
  border: 5px dotted lightgray;
  padding: 10px;
}

.child {
  width: 150px;
  height: 100px;
  border: 3px dotted crimson;
  border-radius: 12px;
  background-color: lightyellow;
}

/* element가 원래 본인 위치를 기준으로 자리 잡음 */
.relative {
  position: relative;
  left: 100px;
  top: 5px;
}
</style>
