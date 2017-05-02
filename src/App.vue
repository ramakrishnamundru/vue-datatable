<template>
    <div id="app">
        <div>
            <datatable title="Demo" :rows="rowdata" :columns="columndata"></datatable>
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
            rowdata: [{
                name: "test1",
                city: "city1"
            }, {
                name: "test2",
                city: "city2"
            }, {
                name: "test3",
                city: "city3"
            }, {
                name: "test4",
                city: "city4"
            }, {
                name: "test5",
                city: "city5"
            }, {
                name: "test1",
                city: "city1"
            }, {
                name: "test2",
                city: "city2"
            }, {
                name: "test3",
                city: "city3"
            }, {
                name: "test4",
                city: "city4"
            }, {
                name: "test5",
                city: "city5"
            }, {
                name: "test1",
                city: "city1"
            }, {
                name: "test2",
                city: "city2"
            }, {
                name: "test3",
                city: "city3"
            }, {
                name: "test4",
                city: "city4"
            }, {
                name: "test5",
                city: "city5"
            }, {
                name: "test1",
                city: "city1"
            }, {
                name: "test2",
                city: "city2"
            }, {
                name: "test3",
                city: "city3"
            }, {
                name: "test4",
                city: "city4"
            }, {
                name: "test5",
                city: "city5"
            }],
            columndata: [ // Array of objects
                {
                    label: 'Name', // Column name
                    field: 'name', // Field name from row
                    // Use dot for nested props
                    // Can be function with row as 1st param
                    numeric: false, // Affects sorting
                    html: false, // Escapes output if false.
                }, {
                    label: 'City', // Column name
                    field: 'city', // Field name from row
                    // Use dot for nested props
                    // Can be function with row as 1st param
                    numeric: false, // Affects sorting
                    html: false, // Escapes output if false.
                }
            ]
        }
    }
}
</script>
