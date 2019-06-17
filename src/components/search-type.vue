<template>
    <div class="form-check">
        <input class="form-check-input" type="checkbox" value="" >
        <label class="form-check-label" for="" :name="name">
            {{name}}
        </label>
    </div>
</template>
<script>
    export default {
        name: 'search-type',
        props: ['name'],
    }
</script>
<style scoped>

</style>