<template>
    <div style="height: 50px; line-height: 50px; border-bottom: 1px solid #ccc; display: flex">
    <div style="width: 200px; padding-left: 30px; font-weight: bold;color: blue">后台管理</div>
    <div style="flex: 1"></div>
    <div style="width: 100px">
        <el-dropdown>
         <span class="el-dropdown-link">
             George<i class="el-icon-arrow-down el-icon--right"></i>
         </span>
            <template #dropdown>
            <el-dropdown-menu slot="dropdown">
                <el-dropdown-item>账号</el-dropdown-item>
                <el-dropdown-item>信息</el-dropdown-item>
                <el-dropdown-item>好友</el-dropdown-item>
                <el-dropdown-item disabled>设置</el-dropdown-item>
                <el-dropdown-item divided>关于</el-dropdown-item>
            </el-dropdown-menu>
            </template>
        </el-dropdown>
    </div>
    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>

</style>