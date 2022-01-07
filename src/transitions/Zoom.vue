<template>
    <mirror
        effect="zoom">
        <template #default>
            <slot/>
        </template>
    </mirror>
</template>

<script>
import Mirror from './Mirror.vue';

export default {
    name: 'Zoom',

    components: { Mirror },
};
</script>
