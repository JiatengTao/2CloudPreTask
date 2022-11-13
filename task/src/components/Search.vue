<template>
    <el-col :xs="0" :sm="20" :lg="6" class="searchbox-container">
        <el-input v-model="input" placeholder="Search for items">
            <template #append>
            <el-button @click="searchKeyword">
                <el-icon size="20" ><search /></el-icon>
            </el-button>
            </template>
        </el-input>
      </el-col>
</template>
<script setup lang="ts">
import { ref } from 'vue'
import { ElMessage, ElMessageBox } from 'element-plus'
import type { Action } from 'element-plus'
const input = ref('')
const fruits = ["apple", "banana", "orange"];
function searchKeyword() {
  const result= fruits.filter((fruit) =>
    fruit.toLowerCase().includes(input.value.toLowerCase())
  );
  if (result.length!=0){
    ElMessageBox.alert(result.toString(), 'Searching for: '+input.value, {
    confirmButtonText: 'OK',
    callback: (action: Action) => {
      ElMessage({
        type: 'info',
        message: `action: ${action}`,
      })
    },
  })
  }else{
    ElMessageBox.alert('No result!', 'Searching for: '+input.value, {
    confirmButtonText: 'OK',
    callback: (action: Action) => {
      ElMessage({
        type: 'info',
        message: `action: ${action}`,
      })
    },
  })
  }
}
</script>