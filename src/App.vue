<template>
    <div id="app">
        <div>
            <datatable></datatable>
        </div>
    </div>
</template>
<script>
import Vue from 'vue';
import DataTable from './DataTable.vue';
export default {
    components: {
        "datatable": DataTable
    },
    data() {
        return {

        }
    }
}
</script>
