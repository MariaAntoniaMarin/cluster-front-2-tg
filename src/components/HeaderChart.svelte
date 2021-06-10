<canvas id='myChart' width='100' height='5'></canvas>

<script>
    fetch('/DataHeaderChart.json')
        .then(response => response.json())
        .then(json => {
            drawChart(json);
        });

    function drawChart(json) {
        let ctx = document.getElementById('myChart');
        let myChart = new Chart(ctx, {
            type: 'bubble',
            data: {
                datasets: [{
                    data: json['clus_1'],
                    backgroundColor: 'rgb(0, 255, 127)'
                }, 
                {
                    data: json['clus_2'],
                    backgroundColor: 'rgb(255, 69, 0)'
                }]
            },
            options: {
                scales: {
                    xAxes: [{
                        display: false
                    }],
                    yAxes: [{
                        display: false
                    }]
                },
                legend: {
                    display: false
                },
                responsive: true, 
                maintainAspectRatio: false,
                tooltips: {
                    enabled: false
                }
            }
        });
    }
</script>
