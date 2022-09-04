
<template>
    <div>
        <el-menu
                style="width: 200px; min-height: 100vh"
                default-active="2"
                class="el-menu-vertical-demo"
                :collapse="isCollapse"
                @open="handleOpen"
                @close="handleClose">
        >
            <el-sub-menu index="1">

                <template #title>
                    <el-icon><CirclePlusFilled /></el-icon>
                    <span>导航</span>
                </template>
                    <el-menu-item index="1-1">item three</el-menu-item>
            </el-sub-menu>
            <el-menu-item index="2">
                <el-icon><icon-menu /></el-icon>
                <template #title>管理</template>
            </el-menu-item>
            <el-menu-item index="3" disabled>
                <el-icon><document /></el-icon>
                <template #title>设置</template>
            </el-menu-item>
            <el-menu-item index="4">
                <el-icon><setting /></el-icon>
                <template #title>关于</template>
            </el-menu-item>
        </el-menu>
    </div>
</template>

<script>
    export default {
        name: "Aside"
    }
</script>

<style scoped>

</style>