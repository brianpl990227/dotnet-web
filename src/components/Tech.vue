<template>
    <div class="p-10">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
            <div>
                <h1 class="text-5xl text-center">¿Qué es .Net?</h1>
                <p class="mt-4">.NET es una plataforma de propósito general que te permite crear y ejecutar aplicaciones
                    para
                    diferentes plataformas, como Windows, Linux, Mac, Android o iOS. Puedes usar varios lenguajes
                    de programación, como C#, Visual Basic, F# o C++, y aprovechar las funcionalidades comunes que te ofrece
                    la biblioteca de clases de .NET. Además, te facilita el desarrollo, la depuración, el despliegue y
                    el mantenimiento de tus aplicaciones con herramientas y servicios integrados. .NET también te garantiza
                    la portabilidad, la productividad, la interoperabilidad, la escalabilidad y la seguridad de tus
                    aplicaciones.</p>
            </div>
            <div class="flex justify-center">
                <img class="h-dotnet" src="/img/dotnet-bot.png" alt="Desarrolladores .Net" />
            </div>
            <div class="mockup-phone">
                <div class="camera"></div>
                <div class="display">
                    <div class="artboard artboard-demo phone-1">
                        <img src="/img/grupo.jpg" alt="Desarrolladores .Net" />
                    </div>
                </div>
            </div>
            <div>
                <h1 class="text-5xl text-center">Nuestra Comunidad</h1>
                <p class="mt-4">Desarrolladores .Net es un grupo de Telegram que te invita a aprender y compartir
                    conocimientos sobre
                    desarrollo
                    de software con el ambiente de .Net y tecnologías de Javascript. Esta comunidad fue fundada por Brian
                    Pérez
                    López, un desarrollador apasionado por la educación y la innovación, que quiso crear un espacio de
                    interacción,
                    apoyo y retroalimentación entre personas con diferentes niveles de experiencia y conocimiento en
                    desarrollo
                    de
                    software.
                    Al unirte a Desarrolladores .Net, podrás acceder a recursos, tutoriales, consejos, ejemplos y
                    proyectos relacionados con .Net y Javascript, así como fomentar el desarrollo de habilidades, la
                    creatividad
                    y
                    la solución de problemas mediante el uso de herramientas y metodologías actuales. Lo mejor de todo es
                    que
                    Desarrolladores .Net no tiene fines de lucro y se basa en los aportes voluntarios de cada miembro del
                    grupo,
                    lo
                    que hace que sea una comunidad activa, diversa y solidaria. Para unirte a Desarrolladores .Net, solo
                    necesitas
                    tener una cuenta de Telegram y presionar el botón de abajo. Una vez que ingreses al
                    grupo, puedes presentarte, consultar tus dudas, compartir tus ideas y participar en las actividades que
                    se
                    propongan. También puedes invitar a otras personas que creas que puedan estar interesadas en formar
                    parte de
                    esta comunidad. No importa si eres principiante o experto, si te gusta .Net o Javascript, si quieres
                    desarrollar
                    aplicaciones web, móviles o de escritorio. En Desarrolladores .Net encontrarás un lugar para ti.
                </p>
                <div class="flex justify-center">
                    <button @click="redirect('https://t.me/DotNetDesarrolladoresGrupo')" class="btn btn-primary mt-6 normal-case">
                        Unirme a la comunidad
                        <TelegramIcon></TelegramIcon>
                    </button>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import TelegramIcon from "./icons/TelegramIcon.vue";

const redirect = url => {
    window.open(url)
}

</script>