<template>
  <div>
    <apexchart
      type="bar"
      height="280"
      :options="chartOptions"
      :series="series"
    ></apexchart>
  </div>
</template>

<script>
export default {
  name: 'myChart',
  data() {
    return {
      series: [
        {
          data: [210, 220, 100],
        },
      ],
      chartOptions: {
        grid: {
          show: false,
        },

        title: {
          text: 'example chart',
          align: 'left',
          margin: 10,
          offsetX: 0,
          offsetY: 0,
          floating: false,
          style: {
            fontSize: '14px',
            fontWeight: 'bold',
            fontFamily: undefined,
            color: '#fff  ',
          },
        },
        fill: {
          colors: ['#9267ff'],
          type: 'gradient',
          gradient: {
            type: 'vertical',
            shadeIntensity: 1,
            stops: [70], // optional, if not defined - uses the shades of same color in series
            inverseColors: false,
            opacityFrom: 1,
            opacityTo: 0,

            colorStops: [],
          },
        },
        chart: {
          show: false,
        },
        tooltip: { enabled: false },
        plotOptions: {
          bar: {
            borderRadius: 15,
            columnWidth: '30%',
            distributed: true,
          },
        },
        dataLabels: {
          enabled: false,
        },
        legend: {
          show: false,
        },
        xaxis: {
          categories: [
            ['210', 'Doe'],
            ['200', 'Smith'],
            ['100', 'Williams'],
          ],
          axisTicks: {
            show: false,
          },
          axisBorder: {
            show: false,
          },
          labels: {
            style: {
              colors: '#fff',
              fontSize: '16px',
              fontWeight: 900,
            },
          },
        },
        yaxis: {
          show: false,
        },
      },
    };
  },
};
</script>
<style lang="scss">
tspan:nth-child(even) {
  font-weight: 800;
  fill: #667cb1;
  font-size: small;
}
</style>
