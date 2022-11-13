<template>
    <div class="demo-collapse">
      <el-collapse accordion>
        <el-collapse-item title=${title} name="1">
          <div>{{text1}}</div>
        </el-collapse-item>
      </el-collapse>
    </div>
  </template>
  
  <script>
  export default(titleInput,textInput) =>{
    name: "Collapse"
    data(); {
        return {
            title:titleInput,
            text1:textInput
        };
    }
}
  </script>
  