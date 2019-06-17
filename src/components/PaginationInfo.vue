<template>
<div class="text-right justify-content-center">
    <template v-if="currentPageRowsLength != 0">
        C 1 по {{currentPageRowsLength}} из {{filteredRowsLength}} записей
    </template>
    <template v-else>
        Ничего не найдено
    </template>
    <template>
         ({{originalRowsLength}} записей всего)
    </template>
</div>
</template>

<script>
export default {
    name: 'PaginationInfo',
    props: {
        currentPageRowsLength: {
            type: Number,
            default: 0
        },
        filteredRowsLength: {
            type: Number,
            default: 0
        },
        originalRowsLength: {
            type: Number,
            default: 0
        }
    },
    data: function () {
        return {

        }
    },
    mounted() {

    },
    methods: {

    }
}
</script>
