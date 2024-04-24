<template>
    <div class="flex flex-col space-y-2">
        <h2 class="text-2xl">Examples in Each Chapter</h2>
        <p>
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Distinctio, reiciendis explicabo facilis nostrum, mollitia vitae atque deserunt ab commodi alias nobis rem incidunt? Expedita officiis neque commodi, sapiente tempora molestias?
        </p>

        <MonacoEditor :options="options" v-model="value" class="h-[150px]" lang="javascript" />
    </div>
</template>
<script setup>
    const options = { 
        readOnly: true,
        lineNumbers: false,
        cursorBlinking: 'solid'
    }
    const value = ref(`
        let a = 'a',
        let b = 
    `);
</script>