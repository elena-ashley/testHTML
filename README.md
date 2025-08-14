<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Intel's Roadmap to Profitability: A Cost Reduction Infographic</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f0f4f8;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
            height: 300px; /* Reverted height */
            max-height: 400px; /* Reverted max-height */
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 350px; /* Reverted height for medium screens */
            }
        }
        .kpi-card {
            background-color: white;
            border-radius: 0.75rem;
            box-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
            padding: 1.5rem;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            min-height: 250px; /* Reverted min-height */
            display: flex;
            flex-direction: column;
        }
        .kpi-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -2px rgb(0 0 0 / 0.1);
        }
        .big-number {
            font-size: 2.5rem;
            font-weight: 900;
            line-height: 1;
            color: #D32F2F;
        }
        .positive-number {
            color: #388E3C;
        }
        .flowchart-item {
            border: 2px solid #01579B;
            background-color: #E1F5FE;
            color: #01579B;
        }
        .bottom-line-box {
            font-size: 0.9rem;
            color: #003F87;
            background-color: #E6F7FF;
            padding: 0.75rem 1.5rem;
            margin-top: 1rem;
            border-radius: 0.75rem;
            box-shadow: 0 2px 4px -1px rgb(0 0 0 / 0.05), 0 1px 2px -1px rgb(0 0 0 / 0.05);
            border-left: 4px solid #4FC3F7;
        }
        .cloudera-help-box {
            font-size: 0.85rem;
            background-color: #F0F8FF;
            border-left: 4px solid #00BFFF;
            padding: 0.75rem;
            margin-top: 1rem;
            border-radius: 0.75rem;
            color: #003F87;
            box-shadow: 0 2px 4px -1px rgb(0 0 0 / 0.05), 0 1px 2px -1px rgb(0 0 0 / 0.05);
        }
        .emphasized-savings {
            font-weight: bold;
            color: #388E3C;
            font-size: 1.1em;
        }
    </style>
</head>
<body class="text-gray-800">

    <header class="bg-white shadow-md">
        <div class="container mx-auto px-6 py-4">
            <h1 class="text-3xl md:text-4xl font-bold text-center text-[#003F87]">Intel's Roadmap to Profitability: Targeting $1B in Cost Reduction</h1>
            <p class="text-center text-lg text-gray-600 mt-2">A Strategic Initiative for Manufacturing and R&D Cost Optimization</p>
        </div>
    </header>

    <main class="container mx-auto px-6 py-8">

        <section id="challenge" class="mb-12">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-2 text-[#003F87]">The 2024 Financial Challenge</h2>
            <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">Intel's 2024 financials reveal a critical need for cost optimization, with significant losses driven by massive capital and R&D expenditures. This plan addresses these challenges head-on.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 text-center">
                <div class="kpi-card">
                    <h3 class="font-semibold text-gray-500">Net Loss</h3>
                    <p class="big-number mt-2">$18.76B</p>
                </div>
                <div class="kpi-card">
                    <h3 class="font-semibold text-gray-500">Capital Expenditures</h3>
                    <p class="big-number mt-2">$23.94B</p>
                </div>
                <div class="kpi-card">
                    <h3 class="font-semibold text-gray-500">R&D Spending</h3>
                    <p class="big-number mt-2">$16.55B</p>
                </div>
                <div class="kpi-card">
                    <h3 class="font-semibold text-gray-500">Gross Margin</h3>
                    <div class="chart-container h-48 max-h-48">
                        <canvas id="grossMarginChart"></canvas>
                    </div>
                </div>
            </div>
        </section>

        <hr class="my-12 border-gray-300">

        <section id="strategy-overview" class="mb-12">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-8 text-[#003F87]">A 9-Point Strategic Response For IDM 2.0 Efficiency</h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 text-center">
                <div class="flowchart-item p-4 rounded-lg font-semibold">⚙️ Predictive Maintenance</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">👁️ Quality Control & Inspection</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">🤖 Robotics & Automation</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">🌐 Digital Twins</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">💡 Energy Efficiency</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">🏗️ Additive Manufacturing</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">🔗 ERP + MES Integration</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">🚚 Supply Chain Optimization</div>
                <div class="flowchart-item p-4 rounded-lg font-semibold">🎨 Mass Customization</div>
            </div>
        </section>

        <hr class="my-12 border-gray-300">

        <section id="manufacturing-excellence">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-2 text-[#003F87]">Pillar 1: Manufacturing & Operational Excellence</h2>
            <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">Optimizing the core of Intel's production through smarter, more efficient factory floor operations to boost yield and reduce direct operating costs.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Predictive Maintenance - 1B Burn Rate</h3>
                        <p class="text-gray-600 mb-4">By predicting equipment failures before they occur, Intel can drastically cut costly unplanned production stops, leading to an estimated <span class="emphasized-savings">$150 million in annual savings</span> and extending asset lifespan.</p>
                        <div class="chart-container">
                            <canvas id="downtimeChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Reduces OpEx (maintenance, scrap), improves Gross Margins (higher uptime, less waste), and supports Revenue by ensuring consistent production.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Provides a unified data platform to ingest real-time IoT sensor data, run advanced machine learning models for anomaly detection, and deliver actionable insights to prevent downtime.
                        </p>
                    </div>
                </div>
                <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Quality Control & Inspection</h3>
                        <p class="text-gray-600 mb-4">Automated AI inspection detects microscopic defects far better than the human eye, directly increasing the number of usable chips per wafer and slashing scrap costs.</p>
                        <div class="chart-container">
                            <canvas id="yieldChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Significantly boosts Gross Margins (higher yields, lower COGS) and reduces OpEx (rework, material waste), indirectly supporting Revenue through higher quality products.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Manages vast volumes of image/video data from inspection systems, enables training and deployment of AI/ML models for computer vision, and provides real-time analytics for defect identification.
                        </p>
                    </div>
                </div>
                 <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Robotics & Automation</h3>
                        <p class="text-gray-600 mb-4">Automating repetitive fab tasks increases wafer throughput, reduces labor costs, and virtually eliminates human error for more consistent production.</p>
                        <div class="chart-container">
                            <canvas id="automationChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Directly lowers OpEx (labor, error costs), improves Gross Margins (efficiency), and drives Revenue by increasing production capacity.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Ingests and processes operational data from robotic systems, enables real-time monitoring of automation performance, and supports optimization of robotic workflows through data analytics.
                        </p>
                    </div>
                </div>
                <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">ERP + MES Integration</h3>
                        <p class="text-gray-600 mb-4">Linking business planning systems (ERP) with real-time factory data (MES) provides total visibility, enabling optimized scheduling and resource use.</p>
                        <div class="chart-container">
                            <canvas id="integrationChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Reduces OpEx (waste, administrative costs), enhances Gross Margins (optimized resource use), and improves Operating Income by streamlining operations.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Provides a robust data platform to integrate and harmonize disparate data from ERP and MES systems, creating a single source of truth for unified analytics and real-time decision-making.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <hr class="my-12 border-gray-300">

        <section id="rd-capex-efficiency">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-2 text-[#003F87]">Pillar 2: R&D and CapEx Efficiency</h2>
            <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">Making multi-billion dollar investments in R&D and new facilities smarter and more efficient by leveraging virtual simulation and rapid prototyping.</p>
             <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Digital Twins</h3>
                        <p class="text-gray-600 mb-4">Simulating entire fabs and processes virtually allows Intel to optimize layouts and debug new technologies before spending billions on physical construction and R&D runs.</p>
                        <div class="chart-container">
                            <canvas id="digitalTwinChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Directly reduces Capital Expenditures (optimized investments) and R&D Spending (fewer physical iterations), improving overall Net Loss.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Manages and processes massive simulation and real-world data sets, enabling advanced analytics and machine learning for predictive modeling and optimization of digital twin scenarios.
                        </p>
                    </div>
                </div>
                 <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Additive Manufacturing (3D Printing)</h3>
                        <p class="text-gray-600 mb-4">3D printing custom tools, fixtures, and prototype parts in-house drastically cuts lead times from weeks to days, accelerating R&D cycles and reducing reliance on external suppliers.</p>
                        <div class="chart-container">
                            <canvas id="additiveChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Lowers R&D Spending (faster, cheaper prototyping) and reduces OpEx (tooling, spare parts), contributing to a healthier Operating Income.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Stores and analyzes complex design files and sensor data from 3D printers, enabling data-driven optimization of print parameters, material usage, and quality control for additive processes.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <hr class="my-12 border-gray-300">

        <section id="foundational-cost-control">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-2 text-[#003F87]">Pillar 3: Foundational Cost Control</h2>
            <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">Strengthening the bottom line by systematically reducing energy costs and optimizing the complex global supply chain that feeds Intel's fabs.</p>
             <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Energy Efficiency & Sustainability</h3>
                        <p class="text-gray-600 mb-4">Semiconductor fabs are huge energy consumers. AI-powered monitoring can identify and eliminate waste, directly cutting one of the largest operational costs.</p>
                        <div class="chart-container">
                            <canvas id="energyChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Directly reduces OpEx (utility bills) and improves Gross Margins (lower COGS), contributing to a positive Operating Income.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Ingests and analyzes real-time energy consumption data from across the fab, applies AI to detect inefficiencies and predict optimal usage, and supports sustainability reporting.
                        </p>
                    </div>
                </div>
                 <div> <!-- Wrapper div for KPI card, Bottom Line box, and Cloudera help box -->
                    <div class="kpi-card">
                        <h3 class="font-bold text-xl mb-2 text-[#00579B]">Supply Chain Optimization</h3>
                        <p class="text-gray-600 mb-4">Using AI to forecast demand and optimize inventory prevents costly material shortages or overstocking, while streamlining logistics to reduce transport costs.</p>
                        <div class="chart-container">
                            <canvas id="supplyChainChart"></canvas>
                        </div>
                    </div>
                    <div class="bottom-line-box">
                        <p>
                            **Bottom Line Effect:** Reduces OpEx (inventory holding, logistics) and improves Gross Margins (lower material costs), positively impacting Operating Income.
                        </p>
                    </div>
                    <div class="cloudera-help-box">
                        <p>
                            **How Cloudera Can Help:** Integrates diverse supply chain data (demand, inventory, logistics, supplier performance) to power advanced forecasting models and optimize material flow, reducing costs and improving resilience.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <hr class="my-12 border-gray-300">

        <section id="projected-impact" class="mb-12">
            <h2 class="text-2xl md:text-3xl font-bold text-center mb-2 text-[#003F87]">Projected Financial Impact</h2>
            <p class="text-center text-gray-600 mb-8 max-w-3xl mx-auto">The cumulative effect of these initiatives is a significant projected improvement in key financial metrics, turning losses into profitability and strengthening gross margins.</p>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                 <div class="kpi-card">
                    <h3 class="font-bold text-xl mb-2 text-[#00579B]">Path to Positive Operating Income</h3>
                    <p class="text-gray-600 mb-4">Reduced operational expenses from higher efficiency, less waste, and lower energy costs can reverse the operating loss.</p>
                    <div class="chart-container">
                        <canvas id="operatingIncomeChart"></canvas>
                    </div>
                </div>
                 <div class="kpi-card">
                    <h3 class="font-bold text-xl mb-2 text-[#00579B]">Strengthening Gross Margins</h3>
                    <p class="text-gray-600 mb-4">A lower cost of goods sold (COGS) from higher yields and a more efficient supply chain directly translates to healthier margins.</p>
                    <div class="chart-container">
                        <canvas id="marginImprovementChart"></canvas>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <footer class="bg-white mt-12">
        <div class="container mx-auto px-6 py-4 text-center text-gray-600">
            <p>&copy; 2025 Hypothetical Intel Strategic Plan. For illustrative purposes only.</p>
            <p class="text-sm mt-1">This infographic was generated to visualize data from the cost-reduction plan. No SVG or Mermaid JS was used; all visualizations are rendered via the HTML Canvas element.</p>
        </div>
    </footer>

    <script>
        const brilliantBlues = {
            primary: '#007BFF',
            secondary: '#00BFFF',
            dark: '#003F87',
            light: '#E1F5FE',
            accent1: '#4FC3F7',
            accent2: '#81D4FA',
            positive: '#388E3C',
            negative: '#D32F2F',
            neutral: '#78909C'
        };

        const tooltipConfig = {
            plugins: {
                tooltip: {
                    callbacks: {
                        title: function(tooltipItems) {
                            const item = tooltipItems[0];
                            let label = item.chart.data.labels[item.dataIndex];
                            if (Array.isArray(label)) {
                                return label.join(' ');
                            } else {
                                return label;
                            }
                        }
                    }
                }
            }
        };

        function wrapLabel(str, maxWidth) {
            if (str.length <= maxWidth) {
                return str;
            }
            const words = str.split(' ');
            let lines = [];
            let currentLine = words[0];
            for (let i = 1; i < words.length; i++) {
                if (currentLine.length + words[i].length + 1 < maxWidth) {
                    currentLine += ' ' + words[i];
                } else {
                    lines.push(currentLine);
                    currentLine = words[i];
                }
            }
            lines.push(currentLine);
            return lines;
        }

        document.addEventListener('DOMContentLoaded', function() {
            
            new Chart(document.getElementById('grossMarginChart'), {
                type: 'doughnut',
                data: {
                    labels: ['Gross Margin', 'Cost of Goods Sold'],
                    datasets: [{
                        data: [32.66, 100 - 32.66],
                        backgroundColor: [brilliantBlues.positive, brilliantBlues.light],
                        borderColor: ['#ffffff'],
                        borderWidth: 2
                    }]
                },
                options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        ...tooltipConfig.plugins,
                        legend: { display: false },
                        title: { display: true, text: '2024 Gross Margin (32.66%)' }
                    }
                }
            });

            new Chart(document.getElementById('downtimeChart'), {
                type: 'bar',
                data: {
                    labels: [
                        ['Unplanned Downtime', '$900M ↓ $765M'],
                        ['Maintenance Costs', '$100M ↓ $92.5M']
                    ],
                    datasets: [
                        { label: 'Before', data: [900, 100], backgroundColor: brilliantBlues.neutral },
                        { label: 'After (Target)', data: [765, 92.5], backgroundColor: brilliantBlues.primary }
                    ]
                },
                options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        y: {
                            beginAtZero: true,
                            ticks: {
                                callback: value => '$' + value + 'M',
                                font: { size: 13 } /* Increased font size by 1pt from 12 to 13 */
                            },
                            title: {
                                display: true,
                                text: 'Cost in Millions ($)',
                                font: { size: 13 } /* Increased font size by 1pt from 12 to 13 */
                            }
                        },
                        x: {
                            ticks: {
                                autoSkip: false,
                                font: { size: 13 } /* Increased font size by 1pt from 12 to 13 */
                            }
                        }
                    },
                    plugins: {
                        ...tooltipConfig.plugins,
                        title: { display: true, text: 'Estimated Annual Impact on $1B Burn Rate' },
                        tooltip: {
                            ...tooltipConfig.plugins.tooltip,
                            callbacks: {
                                title: function(tooltipItems) {
                                    const item = tooltipItems[0];
                                    // If the label is an array, take the first element as the main title
                                    return Array.isArray(item.chart.data.labels[item.dataIndex]) ? item.chart.data.labels[item.dataIndex][0] : item.chart.data.labels[item.dataIndex];
                                },
                                label: context => {
                                    const value = context.raw;
                                    const originalLabel = context.chart.data.labels[context.dataIndex];
                                    const dollarInfo = Array.isArray(originalLabel) ? originalLabel[1] : '';
                                    return `${context.dataset.label}: $${value}M ${dollarInfo ? `(${dollarInfo})` : ''}`;
                                }
                            }
                        }
                    }
                }
            });

            new Chart(document.getElementById('yieldChart'), {
                type: 'bar',
                data: {
                    labels: ['First Pass Yield', 'Defect Rate'],
                    datasets: [
                        { label: 'Before', data: [100, 100], backgroundColor: brilliantBlues.neutral },
                        { label: 'After (Target)', data: [100 + 7.5, 100 - 25], backgroundColor: brilliantBlues.positive }
                    ]
                },
                options: { ...tooltipConfig,
                    responsive: true, maintainAspectRatio: false, indexAxis: 'y',
                    scales: { x: { beginAtZero: true, ticks: { callback: value => value + '%', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins,
                        title: { display: true, text: 'Target: 5-10% Yield ↑, 20-30% Defects ↓' },
                         tooltip: { ...tooltipConfig.plugins.tooltip,
                            callbacks: { ...tooltipConfig.plugins.tooltip.callbacks,
                                label: context => `${context.dataset.label}: ${context.formattedValue}%`
                            }
                        }
                    }
                }
            });

            new Chart(document.getElementById('automationChart'), {
                type: 'bar',
                data: {
                    labels: ['Throughput', 'Human Error Rate'],
                    datasets: [{
                        label: 'Change',
                        data: [15, -80],
                        backgroundColor: [brilliantBlues.positive, brilliantBlues.primary],
                    }]
                },
                options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: { y: { ticks: { callback: value => value + '%', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins, legend: { display: false },
                        title: { display: true, text: 'Target: 10-20% Throughput ↑, 80% Error ↓' }
                    }
                }
            });
            
            new Chart(document.getElementById('integrationChart'), {
                type: 'doughnut',
                data: {
                    labels: ['Schedule Adherence', 'Inventory Accuracy', 'Resource Utilization'],
                    datasets: [{
                        data: [90, 95, 100+7.5],
                        backgroundColor: [brilliantBlues.primary, brilliantBlues.accent1, brilliantBlues.accent2],
                        borderColor: '#ffffff',
                        borderWidth: 2
                    }]
                },
                options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { ...tooltipConfig.plugins, legend: { position: 'top', labels: { font: { size: 12 } } },
                        title: { display: true, text: 'Target KPIs (in %)' }
                    }
                }
            });
            
            new Chart(document.getElementById('digitalTwinChart'), {
                type: 'bar',
                data: {
                    labels: [wrapLabel('R&D Iterations', 16), wrapLabel('Time-to-Market', 16), wrapLabel('CapEx Waste', 16)],
                    datasets: [{
                        label: 'Reduction Target',
                        data: [25, 12.5, 3.5],
                        backgroundColor: [brilliantBlues.primary, brilliantBlues.accent1, brilliantBlues.accent2],
                    }]
                },
                options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: { y: { beginAtZero: true, ticks: { callback: value => value + '%', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins, legend: { display: false },
                        title: { display: true, text: 'Target Reductions via Simulation' },
                         tooltip: { ...tooltipConfig.plugins.tooltip,
                            callbacks: { ...tooltipConfig.plugins.tooltip.callbacks,
                                label: context => `${context.raw}% Reduction`
                            }
                        }
                    }
                }
            });
            
             new Chart(document.getElementById('additiveChart'), {
                type: 'bar',
                data: {
                    labels: [wrapLabel('Prototyping Lead Time', 16), wrapLabel('Tooling Cost', 16)],
                    datasets: [
                        { label: 'Before', data: [100, 100], backgroundColor: brilliantBlues.neutral },
                        { label: 'After (Target)', data: [100 - 60, 100 - 30], backgroundColor: brilliantBlues.primary }
                    ]
                },
                options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: { y: { beginAtZero: true, ticks: { callback: value => value + '%', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins,
                        title: { display: true, text: 'Target Reductions via 3D Printing' },
                         tooltip: { ...tooltipConfig.plugins.tooltip,
                            callbacks: { ...tooltipConfig.plugins.tooltip.callbacks,
                                label: context => `${context.dataset.label}: ${context.formattedValue}% of Original`
                            }
                        }
                    }
                }
            });

            new Chart(document.getElementById('energyChart'), {
                type: 'line',
                data: {
                    labels: ['Q1', 'Q2', 'Q3', 'Q4'],
                    datasets: [{
                        label: 'Energy Consumption Per Unit',
                        data: [100, 97, 94, 92],
                        fill: true,
                        borderColor: brilliantBlues.primary,
                        backgroundColor: 'rgba(0, 123, 255, 0.1)',
                        tension: 0.1
                    }]
                },
                 options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: { y: { beginAtZero: false, ticks: { callback: value => value + '%', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins, legend: { display: false },
                        title: { display: true, text: 'Target: 5-10% Annual Energy Reduction' }
                    }
                }
            });
            
            new Chart(document.getElementById('supplyChainChart'), {
                type: 'radar',
                data: {
                    labels: [wrapLabel('Inventory Turnover', 16), wrapLabel('On-Time Delivery', 16), wrapLabel('Logistics Costs', 16), wrapLabel('Lead Times', 16)],
                    datasets: [
                        { label: 'Before', data: [100, 90, 100, 100], borderColor: brilliantBlues.neutral, backgroundColor: 'rgba(120, 144, 156, 0.2)' },
                        { label: 'After (Target)', data: [112.5, 95, 92.5, 85], borderColor: brilliantBlues.positive, backgroundColor: 'rgba(56, 142, 60, 0.2)' }
                    ]
                },
                 options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { ...tooltipConfig.plugins,
                        title: { display: true, text: 'Supply Chain KPI Improvement' },
                        legend: { labels: { font: { size: 12 } } }
                    }
                }
            });

            new Chart(document.getElementById('operatingIncomeChart'), {
                type: 'bar',
                data: {
                    labels: ['Operating Income'],
                    datasets: [{
                        label: '2024 Actual',
                        data: [-11.68],
                        backgroundColor: brilliantBlues.negative,
                    }, {
                        label: 'Projected Future',
                        data: [5],
                        backgroundColor: brilliantBlues.positive,
                    }]
                },
                 options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: { y: { ticks: { callback: value => '$' + value + 'B', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins,
                        title: { display: true, text: 'From Loss to Projected Profit (in $B)' }
                    }
                }
            });
            
            new Chart(document.getElementById('marginImprovementChart'), {
                type: 'bar',
                data: {
                    labels: ['Gross Margin'],
                    datasets: [{
                        label: '2024 Actual',
                        data: [32.66],
                        backgroundColor: brilliantBlues.neutral,
                    }, {
                        label: 'Projected Future',
                        data: [40],
                        backgroundColor: brilliantBlues.positive,
                    }]
                },
                 options: { ...tooltipConfig,
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: { y: { beginAtZero: true, max: 50, ticks: { callback: value => value + '%', font: { size: 12 } } } },
                    plugins: { ...tooltipConfig.plugins,
                        title: { display: true, text: 'Projected Gross Margin Improvement' }
                    }
                }
            })

        });
    </script>
</body>
</html>

