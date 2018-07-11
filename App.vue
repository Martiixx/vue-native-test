<template>
  <view class="container">
    <text class="text-color-primary" v-bind:on-press="handleBtnPress">{{text}}</text>
    <text-input
        :style="{height: 40, borderColor: 'gray', borderWidth: 1}"
        v-model="text"
      />
    </view>
</template>

<script>
export default {
  data: function() {
    return {
      model: {
      },
      message: "Hello World asdasd asda sdasda",
      text: ''
    };
  },
  methods: {
    handleBtnPress: function() {
      alert('probando cambios' + this.text);
    }
  }
};
</script>
<style>
.container {
  background-color: white;
  align-items: center;
  justify-content: center;
  flex: 1;
}
.text-color-primary {
  color: blue;
}
</style>
