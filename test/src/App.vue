<template>
    <div>
        <div style="display: flex;">
            <Select></Select>
        </div>
        <div style="height: 50px;">
            <Check></Check>
        </div>
        <div>
          <Table></Table>
        </div>
        
    </div>
</template>

<script setup>
import Select from './components/Select.vue';
import Table from './components/Table.vue';
import Check from './components/Check.vue';
</script>