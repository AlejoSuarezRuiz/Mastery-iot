<template>
    <div>
        <div id="chart">
            <!-- <apexchart type=radialBar height=350 :options="chartOptions" :series="series" /> -->
            <DoughnutChart :percent="25" />
        </div>
        <div class="num-data">
            <slot></slot>
        </div>
    </div>
</template>

<style>

</style>

<script>
    import DoughnutChart from 'vue-doughnut-chart'

    export default {
        components: {
            DoughnutChart
        }
    }
</script>