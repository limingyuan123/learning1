<!-- 左侧菜单 -->
<template>
  <div>
    <el-row class="tac">
      <el-col>
        <el-menu
          default-active="2"
          class="el-menu-vertical-demo"
          @open="handleOpen"
          @close="handleClose"
        >
        <!-- 前端目录树 -->
          <el-sub-menu index="1">
            <template #title>
              <el-icon><setting /></el-icon>
              <span>前端</span>
            </template>
            <el-menu-item index="1-1">
              <el-icon><icon-menu /></el-icon>
              <span>HTML/CSS</span>
            </el-menu-item>
            <el-menu-item index="1-2">
              <el-icon><setting /></el-icon>
              <span>VUE</span>
            </el-menu-item>
            <el-menu-item index="1-3">
              <el-icon><setting /></el-icon>
              <span>React</span>
            </el-menu-item>
          </el-sub-menu>

        <!-- 后端目录树 -->
          <el-sub-menu index="2">
            <template #title>
              <el-icon><setting /></el-icon>
              <span>后端</span>
            </template>
            <el-menu-item index="2-1">
              <el-icon><setting /></el-icon>
              <span>NodeJS</span>
            </el-menu-item>
            <el-menu-item index="2-2">
              <el-icon><setting /></el-icon>
              <span>Spring Boot</span>
            </el-menu-item>
          </el-sub-menu>

        <!-- 数据库目录树 -->
          <el-sub-menu index="3">
            <template #title>
              <el-icon><setting /></el-icon>
              <span>数据库</span>
            </template>            
            <el-menu-item index="3-1">
              <el-icon><setting /></el-icon>
              <span>MongoDB</span>
            </el-menu-item>
            <el-menu-item index="3-2">
              <el-icon><setting /></el-icon>
              <span>MySQL</span>
            </el-menu-item>
          </el-sub-menu>

        <!-- 网站开发目录树 -->
          <el-sub-menu index="4">
            <template #title>
              <el-icon><setting /></el-icon>
              <span>网站开发</span>
            </template>            
            <el-menu-item index="4-1">
              <el-icon><setting /></el-icon>
              <span>前后端</span>
            </el-menu-item>
            <el-menu-item index="4-2">
              <el-icon><setting /></el-icon>
              <span>网站协议</span>
            </el-menu-item>
          </el-sub-menu>

          
        </el-menu>
      </el-col>
    </el-row>
  </div>
</template>

<script lang="ts" setup>
import {
  Menu as IconMenu,
  Setting,
} from '@element-plus/icons-vue'



const handleOpen = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
const handleClose = (key: string, keyPath: string[]) => {
  console.log(key, keyPath)
}
</script>

<style scoped>

</style>
