<script>
  import { Pie } from 'vue-chartjs'
  
  export default {
    extends: Pie,
    data() {
      return {
        chartData: {
          labels: ['January', 'February'],
          datasets: [
            {
              label: 'Data One',
              backgroundColor: '#f87979',
              data: [40, 20],
            },
          ],
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
        },
      }
    },
    mounted() {
      this.renderChart(this.chartData, this.options)
    },
  }
  </script>