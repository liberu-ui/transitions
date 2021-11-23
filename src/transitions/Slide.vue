<template>
    <mirror v-bind="$attrs"
        effect="slide">
        <template #default>
            <slot/>
        </template>
    </mirror>
</template>

<script>
import Mirror from './Mirror.vue';

export default {
    name: 'Slide',

    components: { Mirror },
}

</script>
