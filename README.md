<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio de Servicios | DIRECCIÓN DE LABORATORIOS SEDE BOGOTÁ UNAL</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f1f1f1;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 500px;
            margin-left: auto;
            margin-right: auto;
            height: 320px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 400px;
            }
        }
        .flow-arrow-h {
            display: none;
        }
         @media (min-width: 1024px) {
            .flow-arrow-h {
                display: flex;
                align-items: center;
                justify-content: center;
                font-size: 2.5rem;
                color: #4d8fac;
                padding: 0 1rem;
            }
        }
        .flow-arrow-v {
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2.5rem;
            color: #4d8fac;
            padding: 1rem 0;
            transform: rotate(90deg);
        }
        @media (min-width: 1024px) {
            .flow-arrow-v {
                display: none;
            }
        }
    </style>
</head>
<body class="text-gray-800">

    <!-- Palette: Brilliant Blues (#003f5c, #4d8fac, #9ad2e6, #f1f1f1) -->
    <!-- Plan: 1. Header, 2. Core Services (Donut Chart), 3. Workflow (HTML/CSS Flowchart), 4. Impact (Stacked Bar Chart), 5. User Breakdown (Pie Chart) & Efficiency (H. Bar Chart), 6. Footer. -->
    <!-- Visualizations Justification: Donut (Composition), Flowchart (Process), Stacked Bar (Composition/Comparison), Pie (Simple Composition), H. Bar (Comparison/Ranking). All using Chart.js or styled HTML/CSS. NO SVG. NO MERMAID JS. -->

    <header class="bg-white shadow-lg p-6 md:p-10 text-center">
        <h1 class="text-4xl md:text-5xl font-black" style="color: #003f5c;">Laboratorio de Biotecnología Aplicada</h1>
        <p class="text-xl md:text-2xl font-light mt-2" style="color: #4d8fac;">Facultad de Ciencias - Universidad Nacional de Colombia</p>
        <p class="max-w-4xl mx-auto mt-4 text-gray-600">Apoyamos la docencia, investigación y extensión a través de servicios analíticos especializados. Nuestra infraestructura y equipo experto garantizan resultados precisos y confiables para la comunidad académica y el sector industrial.</p>
    </header>

    <main class="container mx-auto p-4 md:p-8">
        
        <section id="kpis" class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center my-8">
            <div class="bg-white rounded-lg shadow-md p-6">
                <p class="text-5xl font-extrabold" style="color: #003f5c;">+1,200</p>
                <p class="text-lg font-medium text-gray-700 mt-2">Muestras Procesadas en 2024</p>
            </div>
            <div class="bg-white rounded-lg shadow-md p-6">
                <p class="text-5xl font-extrabold" style="color: #003f5c;">+60</p>
                <p class="text-lg font-medium text-gray-700 mt-2">Proyectos de Investigación Apoyados</p>
            </div>
            <div class="bg-white rounded-lg shadow-md p-6">
                <p class="text-5xl font-extrabold" style="color: #003f5c;">98%</p>
                <p class="text-lg font-medium text-gray-700 mt-2">Índice de Satisfacción del Usuario</p>
            </div>
        </section>

        <section id="services" class="my-12">
            <div class="bg-white rounded-lg shadow-md p-6 md:p-8">
                <h2 class="text-3xl font-bold text-center mb-2" style="color: #003f5c;">Nuestro Portafolio de Servicios</h2>
                <p class="text-center text-gray-600 max-w-3xl mx-auto mb-8">Ofrecemos un amplio rango de análisis y ensayos. A continuación, se presenta la distribución de la demanda de nuestros servicios más solicitados, reflejando nuestras áreas de mayor especialización y aporte a la comunidad.</p>
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 items-center">
                    <div class="chart-container">
                        <canvas id="servicesDonutChart"></canvas>
                    </div>
                    <div class="space-y-4">
                        <div class="p-4 border-l-4" style="border-color: #003f5c;">
                            <h3 class="font-bold text-lg">Secuenciación de ADN (Sanger)</h3>
                            <p class="text-gray-600 text-sm">Análisis de secuencias para validación de construcciones, identificación de mutaciones y genotipado.</p>
                        </div>
                        <div class="p-4 border-l-4" style="border-color: #4d8fac;">
                            <h3 class="font-bold text-lg">Análisis de Expresión Génica (qPCR)</h3>
                            <p class="text-gray-600 text-sm">Cuantificación relativa y absoluta de la expresión de genes de interés en diversas muestras biológicas.</p>
                        </div>
                        <div class="p-4 border-l-4" style="border-color: #9ad2e6;">
                            <h3 class="font-bold text-lg">Análisis Proteómico (Espectrometría)</h3>
                            <p class="text-gray-600 text-sm">Identificación y cuantificación de proteínas para estudios de perfiles proteicos complejos.</p>
                        </div>
                         <div class="p-4 border-l-4" style="border-color: #f7a844;">
                            <h3 class="font-bold text-lg">Cultivo Celular y Bioensayos</h3>
                            <p class="text-gray-600 text-sm">Mantenimiento de líneas celulares y ejecución de ensayos de citotoxicidad y proliferación.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="workflow" class="my-12">
            <h2 class="text-3xl font-bold text-center mb-2" style="color: #003f5c;">Nuestro Flujo de Trabajo</h2>
            <p class="text-center text-gray-600 max-w-3xl mx-auto mb-8">Hemos estandarizado nuestro proceso para garantizar eficiencia, transparencia y calidad en cada etapa. Este flujo aplica para todos nuestros usuarios, asegurando una experiencia consistente y profesional.</p>
            <div class="flex flex-col lg:flex-row justify-center items-center gap-4">
                <div class="bg-white rounded-lg shadow-md p-6 text-center w-full max-w-xs flex-shrink-0">
                    <div class="text-4xl font-extrabold mb-2" style="color: #003f5c;">1</div>
                    <h3 class="font-bold text-lg">Solicitud</h3>
                    <p class="text-sm text-gray-600">El usuario diligencia y envía el formulario de solicitud de servicio.</p>
                </div>
                <div class="flow-arrow-v lg:flow-arrow-h">➔</div>
                <div class="bg-white rounded-lg shadow-md p-6 text-center w-full max-w-xs flex-shrink-0">
                    <div class="text-4xl font-extrabold mb-2" style="color: #003f5c;">2</div>
                    <h3 class="font-bold text-lg">Revisión y Cotización</h3>
                    <p class="text-sm text-gray-600">El laboratorio revisa la viabilidad y envía la cotización formal.</p>
                </div>
                <div class="flow-arrow-v lg:flow-arrow-h">➔</div>
                <div class="bg-white rounded-lg shadow-md p-6 text-center w-full max-w-xs flex-shrink-0">
                    <div class="text-4xl font-extrabold mb-2" style="color: #003f5c;">3</div>
                    <h3 class="font-bold text-lg">Pago y Muestras</h3>
                    <p class="text-sm text-gray-600">Se confirma el pago y se reciben las muestras debidamente identificadas.</p>
                </div>
                <div class="flow-arrow-v lg:flow-arrow-h">➔</div>
                <div class="bg-white rounded-lg shadow-md p-6 text-center w-full max-w-xs flex-shrink-0">
                    <div class="text-4xl font-extrabold mb-2" style="color: #003f5c;">4</div>
                    <h3 class="font-bold text-lg">Análisis</h3>
                    <p class="text-sm text-gray-600">Se procesan las muestras siguiendo protocolos estandarizados de alta calidad.</p>
                </div>
                 <div class="flow-arrow-v lg:flow-arrow-h">➔</div>
                <div class="bg-white rounded-lg shadow-md p-6 text-center w-full max-w-xs flex-shrink-0">
                    <div class="text-4xl font-extrabold mb-2" style="color: #003f5c;">5</div>
                    <h3 class="font-bold text-lg">Entrega de Resultados</h3>
                    <p class="text-sm text-gray-600">Se envían los resultados y el informe final al correo del usuario.</p>
                </div>
            </div>
        </section>

        <section id="impact" class="grid grid-cols-1 lg:grid-cols-2 gap-8 my-12">
            <div class="bg-white rounded-lg shadow-md p-6 md:p-8">
                <h3 class="text-2xl font-bold text-center mb-2" style="color: #003f5c;">Perfil de Nuestros Usuarios</h3>
                 <p class="text-center text-gray-600 max-w-3xl mx-auto mb-6">Nuestros servicios son un pilar fundamental tanto para la comunidad académica de la UNAL como para el sector externo, fomentando la sinergia entre la investigación, la docencia y la industria.</p>
                <div class="chart-container h-80 md:h-96">
                    <canvas id="userProfileChart"></canvas>
                </div>
            </div>
            <div class="bg-white rounded-lg shadow-md p-6 md:p-8">
                <h3 class="text-2xl font-bold text-center mb-2" style="color: #003f5c;">Distribución Anual de Solicitudes</h3>
                 <p class="text-center text-gray-600 max-w-3xl mx-auto mb-6">El gráfico muestra el balance entre las solicitudes provenientes de la propia universidad y las de clientes externos, evidenciando nuestro rol dual como centro de soporte académico y proveedor de servicios especializados.</p>
                <div class="chart-container h-80 md:h-96">
                    <canvas id="userDistributionChart"></canvas>
                </div>
            </div>
        </section>
        
        <section id="efficiency" class="my-12">
             <div class="bg-white rounded-lg shadow-md p-6 md:p-8">
                 <h2 class="text-3xl font-bold text-center mb-2" style="color: #003f5c;">Eficiencia y Tiempos de Entrega</h2>
                 <p class="text-center text-gray-600 max-w-3xl mx-auto mb-8">La optimización de nuestros procesos nos permite ofrecer tiempos de respuesta competitivos. A continuación se muestra el tiempo promedio de entrega (en días hábiles) para nuestros principales servicios.</p>
                 <div class="chart-container h-96 md:h-[500px] max-w-4xl">
                     <canvas id="deliveryTimeChart"></canvas>
                 </div>
            </div>
        </section>

    </main>
    
    <footer class="bg-white mt-12 p-8 text-center border-t-4" style="border-color: #003f5c;">
        <h2 class="text-2xl font-bold" style="color: #003f5c;">Contáctenos</h2>
        <p class="text-gray-600 mt-2">¿Interesado en nuestros servicios? No dude en ponerse en contacto.</p>
        <div class="mt-4 text-gray-700">
            <p><strong>Coordinador:</strong> Dr. Juan Pérez</p>
            <p><strong>Correo:</strong> labbiotec_fcbog@unal.edu.co</p>
            <p><strong>Teléfono:</strong> (+57) 601 316 5000 Ext. 12345</p>
            <p><strong>Ubicación:</strong> Edificio 421, Oficina 210, Campus Bogotá</p>
        </div>
    </footer>

    <script>
        function wrapLabel(str, maxLen) {
            if (str.length <= maxLen) {
                return str;
            }
            const words = str.split(' ');
            const lines = [];
            let currentLine = '';
            for (const word of words) {
                if ((currentLine + word).length > maxLen && currentLine.length > 0) {
                    lines.push(currentLine.trim());
                    currentLine = '';
                }
                currentLine += word + ' ';
            }
            lines.push(currentLine.trim());
            return lines;
        }
        
        const tooltipTitleCallback = (tooltipItems) => {
            const item = tooltipItems[0];
            let label = item.chart.data.labels[item.dataIndex];
            if (Array.isArray(label)) {
              return label.join(' ');
            } else {
              return label;
            }
        };

        const globalChartOptions = {
            responsive: true,
            maintainAspectRatio: false,
            plugins: {
                legend: {
                    position: 'bottom',
                     labels: {
                        font: {
                            family: 'Inter',
                            size: 12,
                        }
                    }
                },
                tooltip: {
                    callbacks: {
                        title: tooltipTitleCallback
                    },
                    titleFont: { family: 'Inter' },
                    bodyFont: { family: 'Inter' }
                }
            },
            
        };

        const brilliantBluesPalette = ['#003f5c', '#4d8fac', '#9ad2e6', '#f7a844', '#a05195'];

        new Chart(document.getElementById('servicesDonutChart'), {
            type: 'doughnut',
            data: {
                labels: ['Secuenciación de ADN', 'Análisis de Expresión Génica (qPCR)', 'Análisis Proteómico', 'Cultivo Celular y Bioensayos'],
                datasets: [{
                    label: 'Distribución de Servicios',
                    data: [40, 25, 20, 15],
                    backgroundColor: brilliantBluesPalette,
                    borderColor: '#f1f1f1',
                    borderWidth: 4
                }]
            },
            options: {
                ...globalChartOptions,
                 plugins: {
                    ...globalChartOptions.plugins,
                    legend: {
                        position: 'right',
                        labels: {
                            font: { family: 'Inter', size: 12},
                            boxWidth: 20
                        }
                    }
                }
            }
        });

        new Chart(document.getElementById('userProfileChart'), {
            type: 'bar',
            data: {
                labels: ['Usuarios Internos', 'Usuarios Externos'],
                datasets: [
                    {
                        label: 'Investigación / I+D',
                        data: [75, 55],
                        backgroundColor: '#003f5c',
                    },
                    {
                        label: 'Docencia / Academia',
                        data: [25, 10],
                        backgroundColor: '#4d8fac',
                    },
                    {
                        label: 'Industria',
                        data: [0, 35],
                        backgroundColor: '#9ad2e6',
                    }
                ]
            },
            options: {
                ...globalChartOptions,
                scales: {
                    x: {
                        stacked: true,
                        ticks: { font: { family: 'Inter' } }
                    },
                    y: {
                        stacked: true,
                        beginAtZero: true,
                        title: { display: true, text: 'Número de Solicitudes', font: { family: 'Inter' } },
                        ticks: { font: { family: 'Inter' } }
                    }
                }
            }
        });

        new Chart(document.getElementById('userDistributionChart'), {
            type: 'pie',
            data: {
                labels: ['Usuarios Internos UNAL', 'Usuarios Externos'],
                datasets: [{
                    label: 'Distribución Anual',
                    data: [65, 35],
                    backgroundColor: ['#003f5c', '#9ad2e6'],
                    borderColor: '#f1f1f1',
                    borderWidth: 4
                }]
            },
            options: { ...globalChartOptions }
        });

        const deliveryLabelsRaw = [
            'Análisis Bioinformático Básico', 
            'Cultivo Celular (Pase Estándar)', 
            'Análisis de Expresión Génica (qPCR)', 
            'Secuenciación de ADN (Placa 96 pocillos)', 
            'Análisis Proteómico (Gel 2D)'
        ];
        const deliveryLabelsWrapped = deliveryLabelsRaw.map(label => wrapLabel(label, 25));

        new Chart(document.getElementById('deliveryTimeChart'), {
            type: 'bar',
            data: {
                labels: deliveryLabelsWrapped,
                datasets: [{
                    label: 'Días Hábiles',
                    data: [3, 5, 7, 10, 15],
                    backgroundColor: '#4d8fac',
                    borderColor: '#003f5c',
                    borderWidth: 1
                }]
            },
            options: {
                ...globalChartOptions,
                indexAxis: 'y',
                plugins: {
                    legend: {
                        display: false
                    },
                     tooltip: {
                        callbacks: {
                           title: tooltipTitleCallback
                        }
                    }
                },
                scales: {
                    x: {
                        beginAtZero: true,
                        title: { display: true, text: 'Tiempo Promedio de Entrega (Días Hábiles)', font: { family: 'Inter' }},
                        ticks: { font: { family: 'Inter' }}
                    },
                    y: {
                        ticks: { font: { family: 'Inter', size: 12 }}
                    }
                }
            }
        });

    </script>
</body>
</html>
