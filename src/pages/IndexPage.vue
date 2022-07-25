<template>
  <q-page class="column items-center justify-center">
    <span>마우스 이벤트</span>
    <span>@click</span>
    <input type="text" @click="handleEvent" />
    <span>@dblclick</span>
    <input type="text" @dblclick="handleEvent" />
    <span>@mouseover</span>
    <input type="text" @mouseover="handleEvent" />
    <span>@mouseout</span>
    <input type="text" @mouseout="handleEvent" />
    <span>@mouseup</span>
    <input type="text" @mouseup="handleEvent" />
    <span>@mousemove</span>
    <input type="text" @mousemove="handleEvent" />
    <span>@contextmenu</span>
    <input type="text" @contextmenu="handleEvent" />
    <br />
    <span>키 이벤트</span>
    <span>@keydown</span>
    <input type="text" @keydown="handleEvent" />
    <span>@keyup</span>
    <input type="text" @keyup="handleEvent" />
    <span>@keypress</span>
    <input type="text" @keypress="handleEvent" />
    <br />
    <span>폼 이벤트</span>
    <span>@submit</span>
    <form @submit="handleEvent">
      <input type="text" />
      <input type="submit" />
    </form>
    <span>@change</span>
    <input type="text" @change="handleEvent" />
    <span>@focus</span>
    <input type="text" @focus="handleEvent" />
    <span>@blur</span>
    <input type="text" @blur="handleEvent" />
    <span>@select: 드래그하여 선택</span>
    <input type="text" @select="handleEvent" value="input text" />
    <span>@reset</span>
    <form @reset="handleEvent">
      <input type="text" />
      <input type="reset" />
    </form>
    <div>commit test</div>
  </q-page>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
  setup() {
    const handleEvent = () => {
      console.log("mouse event triggered");
    };

    return {
      handleEvent,
    };
  },
});
</script>
