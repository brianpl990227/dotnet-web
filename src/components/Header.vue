<template>
    <div class="relative h-screen w-screen flex flex-col items-center justify-center">
        
        <div class="mockup-code mx-4 w-96">
            <pre data-prefix="$"><code>{{ code.command }}</code></pre>
            <pre data-prefix=">" class="text-warning"><code>{{ code.com }}</code></pre>
            <pre data-prefix=">" class="text-success"><code>{{ code.final }}</code></pre>
        </div>
    </div>
</template>
  
<script setup>
import { ref } from "vue";


const code = ref({
    command: '',
    com: '',
    final: ''
})

const text = 'dotnet run'


const updateCode = async times => {

    console.log(times)
    if (times == 20) {
        return;
    }

    for (let i = 0; i < 10; i++) {
        await wait(0.2)
        code.value.command += text[i]
    }

    if (code.value.command == text) {
        await wait(1)
        code.value.com = 'Compilando...'

        await wait(2)
        code.value.final = 'Desarrolladores .Net'
        await wait(5)
        
            code.value = {
                command: '',
                com: '',
                final: ''
            }
        
    }

    setTimeout(updateCode, 100, (times + 1))

}

function wait(seconds) {
    return new Promise(resolve => {
        setTimeout(resolve, seconds * 1000);
    });
}

setTimeout(updateCode, 100, 0)


</script>