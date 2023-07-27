<script>
export default {
    props: ['biodata']
}
</script>

<template>
    <div class="bg-white" id="bio">
        <div class="mx-2 pt-10">
            <div class="mx-auto max-w-max overflow-hidden rounded-xl hover:shadow-lg transition">
                <img class="hover:scale-125 transition-all hover:opacity-75" src="/img/kkrdwn.jpg" alt="KKRDWN_" width="300">
            </div>
        </div>
        <div class="py-8">
            <h2 class="text-center font-semibold text-2xl my-2">Biodata</h2>
            <table class="mx-auto">
                <tr v-for="data in biodata">
                    <td class="px-1">{{ data[0] }}</td>
                    <td class="px-1">:</td>
                    <td class="px-1">{{ data[1] }}</td>
                </tr>
            </table>
        </div>
    </div>
</template>