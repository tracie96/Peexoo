<template>
    <vc-calendar :attributes='attributes' :masks="{ title: 'MMMM', weekdays: 'WW' }" :columns="$screens({ default: 1, lg: 3 })" :rows="$screens({ default: 1, lg: 1 })"
        :is-expanded="$screens({ default: true, lg: false })" />
</template>

<script>
    //import TRVLPicker from '@trvl/picker'
    export default {
        name: "calendar-slider",
        components: {

        },
        data: function () {
            return {
                attributes: [
                    {
                        key: 'today',
                        highlight: true,
                        dates: new Date()
                    }
                ]
            }
        },
    }
</script>