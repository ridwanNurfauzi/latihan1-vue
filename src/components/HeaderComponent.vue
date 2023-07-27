<script setup>
</script>

<template>
    <div class="border-black bg-[url(/img/bg.png)] bg-center bg-cover" id="home">
        <div class="bg-slate-100 px-2 py-40 pb-52 bg-opacity-25 backdrop-blur-sm text-gray-800">
            <slot name="title"></slot>
            <slot name="text"></slot>
            <slot name="body"></slot>
        </div>
    </div>
</template>