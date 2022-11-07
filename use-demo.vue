<template>
  <div>
    <locate-picker @change="change">
      <span>{{ locateValue }}</span>
    </locate-picker>
  </div>
</template>

<script>
export default {
  data() {
    return {
      locateValue: '请选择地区',
    };
  },
  methods: {
    change(data) {
      this.locateValue = data.data.join(' ');
    },
  },
};
</script>

<style lang="scss" scoped></style>
