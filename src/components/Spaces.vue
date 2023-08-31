<template>
    <div class="p-10">
        <h1 class="text-5xl text-center">¿Qué te ofrecemos?</h1>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8 mt-6">
            <div class="card bg-slate-800 shadow-xl">
                <figure class="px-10 pt-10">
                   <TelegramHuge></TelegramHuge>
                </figure>
                <div class="card-body items-center text-center">
                    <h2 class="card-title">Comunidad</h2>
                    <p>Una comunidad donde puedes hacer tus preguntas para ayudarnos entre todos a ser mejores profesionales</p>
                    <div class="card-actions">
                        <button @click="redirect('https://t.me/DotNetDesarrolladoresGrupo')" class="btn btn-primary normal-case mt-6">Unirme</button>
                    </div>
                </div>
            </div>
            <div class="card bg-slate-800 shadow-xl">
                <figure class="px-10 pt-10">
                    <Github></Github>
                </figure>
                <div class="card-body items-center text-center">
                    <h2 class="card-title">Repositorio</h2>
                    <p>Una organización de Github donde se guardarán los proyectos con fines didácticos que se desarrollen</p>
                    <div class="card-actions">
                        <button @click="redirect('https://github.com/Desarrolladores-Net')" class="btn btn-primary normal-case mt-6">Ver repositorio</button>
                    </div>
                </div>
            </div>
            <div class="card bg-slate-800 shadow-xl">
                <figure class="px-10 pt-10">
                    <Books></Books>
                </figure>
                <div class="card-body items-center text-center">
                    <h2 class="card-title">Aprendizaje</h2>
                    <p>Un espacio donde encontrarás variedad de PDFs sobre desarrollo de software para el estudio y la superación</p>
                    <div class="card-actions">
                        <button @click="redirect('https://t.me/AprendizajeDotNet')" class="btn btn-primary normal-case">Aprender</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import TelegramHuge from "./icons/TelegramHuge.vue";
import Github from "./icons/Github.vue";
import Books from "./icons/Books.vue";

const redirect = url => {
    window.open(url)
}

</script>