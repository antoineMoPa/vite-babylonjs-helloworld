<template>
  <div class="canvas-container"></div>
</template>

<script>

import App from "../classes/App.ts";

export default {
  name: 'HelloWorld',
  data() {
    return {
      count: 0
    }
  },
  mounted() {
    let canvasContainer = document.querySelectorAll(".canvas-container")[0];
    let app = new App();
    canvasContainer.appendChild(app.canvas);
  }
}
</script>
