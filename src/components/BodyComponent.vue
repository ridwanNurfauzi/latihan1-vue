<script>
export default {
    props: ['biodata']
}
</script>

<template>
    <div class="bg-white" id="bio">
        <div class="mx-2 pt-10">
            <div class="mx-auto max-w-max overflow-hidden rounded-xl hover:shadow-lg transition">
                <img class="hover:scale-125 transition-all hover:opacity-75" src="/img/kkrdwn2.jpg" alt="KKRDWN_"
                    width="300">
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
    <div class="bg-gray-200 px-3 py-3" id="project">
            <h2 class="font-semibold text-2xl text-center mb-10">My Project</h2>
        <div class="flex">
            <div class="flex flex-wrap m-9 mx-auto justify-center">
                <a class="m-5" target="_blank" href="https://ridwannurfauzi.github.io/mediapintar.com/">
                    <div style="width: 300px; height: 150px;" class="bg-white hover:shadow-md rounded-md flex items-center">
                        <div style="width: 100px; height: 100px;"
                            class="rounded-full bg-gray-300 mx-4 bg-[url('https://ridwannurfauzi.github.io/mediapintar.com/icon.png')] bg-center bg-cover">
                        </div>
                        <h2 class="font-semibold text-lg">mediapintar.com</h2>
                    </div>
                </a>
                <a class="m-5" target="_blank" href="https://ridwannurfauzi.github.io/kk/">
                    <div style="width: 300px; height: 150px;" class="bg-white hover:shadow-md rounded-md flex items-center">
                        <div style="width: 100px; height: 100px;"
                            class="rounded-full bg-gray-300 mx-4 bg-[url('https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTJvfqaEGoktbwFoWxaPDKOPJQEwA8wyElM3rGCZRE&s')] bg-center bg-cover">
                        </div>
                        <h2 class="font-semibold text-lg">Galery</h2>
                    </div>
                </a>
                <a class="m-5" target="_blank" href="https://ridwannurfauzi.github.io">
                    <div style="width: 300px; height: 150px;" class="bg-white hover:shadow-md rounded-md flex items-center">
                        <div style="width: 100px; height: 100px;"
                            class="rounded-full bg-gray-300 mx-4 bg-[url('https://ridwannurfauzi.github.io/Ic.png')] bg-center bg-cover">
                        </div>
                        <h2 class="font-semibold text-lg">Web Profile</h2>
                    </div>
                </a>
            </div>
        </div>
</div></template>