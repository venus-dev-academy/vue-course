<script setup>
import { ref, onMounted } from 'vue'

const count = ref(0)

onMounted(() => {
    console.log(count.value)
})

</script>

<template>
    <div>
        <p>This is the sample app.</p>
        <button
            @click="count++"
        >
            click Me
        </button>
        <p>{{ count }}</p>
    </div>
</template>