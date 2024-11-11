<template>
  <div class="check-box">
    <a-checkbox-group v-model:value="state.value1" name="checkboxgroup" :options="checkboxOptions" />
    <PlusOutlined />
  </div>
  </template>
  <script setup>
  import { reactive ,ref} from 'vue';
  import {PlusOutlined} from '@ant-design/icons-vue'

  const checkboxOptions = ['创建时间','设备ID','0.3um','0.5um','1um','3um','5um','10um','流量']

  const state = reactive({
    value1: ['创建时间','设备ID','0.3um','0.5um','1um','3um','5um','10um','流量'],
    value2: ['创建时间'],
    value3: ['设备ID'],
    value4: ['0.3um'],
    value5: ['0.5um'],
    value6: ['1um'],
    value7: ['3um'],
    value8: ['5um'],
    value9: ['10um'],
    value10: ['流量'],

  });
  
  </script>

<style scoped>
.check-box{
  height: 50px;
  width: 100%;
  margin: 20px 0;
  background-color: rgb(216, 215, 215);
  border: 0.2px solid rgb(161, 160, 160);
  text-align: right;
  line-height: 50px;
}
</style>