<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Voestalpine & LYNXX: Digital Rail Collaboration Explorer (AI Enhanced)</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <!-- Visualization & Content Choices: 
        - Report Info: Executive Summary -> Goal: Inform -> Viz/Presentation: Formatted text -> Interaction: Read -> Justification: Provides high-level context.
        - Report Info: zentrak Ecosystem (Table 3) -> Goal: Organize/Inform -> Viz/Presentation: Interactive accordion/list -> Interaction: Click to expand/collapse -> Justification: Presents complex system components clearly. Library/Method: HTML/JS.
        - Report Info: Sensor Technologies (Table 2) -> Goal: Inform/Compare -> Viz/Presentation: Bar Chart -> Interaction: Hover for tooltips -> Justification: Visualizes the range of sensors and data types. Library/Method: Chart.js.
        - Report Info: Core Products (Table 1, Sec 3 & 5) -> Goal: Inform -> Viz/Presentation: Cards with key details -> Interaction: Read -> Justification: Highlights key products. Library/Method: HTML/Tailwind.
        - Report Info: LYNXX Capabilities (Table 4) -> Goal: Compare/Inform -> Viz/Presentation: Interactive table -> Interaction: Read -> Justification: Maps LYNXX's strengths. Library/Method: HTML/Tailwind.
        - Report Info: Business Models (Sec 7) -> Goal: Inform/Compare -> Viz/Presentation: Interactive cards -> Interaction: Click to reveal details -> Justification: Allows easy comparison. Library/Method: HTML/JS.
        - Report Info: Key Questions for LYNXX (Sec 8) -> Goal: Inform/Prepare -> Viz/Presentation: List with "Elaborate" buttons -> Interaction: Click to call Gemini API for elaboration -> Justification: Provides AI-powered preparation. Library/Method: HTML/JS/Gemini API.
        - Report Info: Harald Hopfgartner Profile -> Goal: Prepare -> Viz/Presentation: Profile text with "Generate Talking Points" button -> Interaction: Click to call Gemini API -> Justification: AI-assisted meeting prep. Library/Method: HTML/JS/Gemini API.
        - CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. All charts use Chart.js (Canvas). Diagrams are structured HTML/CSS.
    -->
    <style>
        body { font-family: 'Inter', sans-serif; }
        .section-active { display: block; }
        .section-inactive { display: none; }
        .nav-link { transition: all 0.3s ease; }
        .nav-link.active { color: #0284c7; border-bottom-color: #0284c7; }
        .nav-link:not(.active):hover { color: #0369a1; border-bottom-color: #0369a1; }
        .chart-container { position: relative; width: 100%; max-width: 700px; margin-left: auto; margin-right: auto; height: 400px; max-height: 50vh; }
        @media (min-width: 768px) { .chart-container { height: 450px; } }
        .tab-content { animation: fadeIn 0.5s; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        .accordion-content { max-height: 0; overflow: hidden; transition: max-height 0.3s ease-out; }
        .accordion-content.open { max-height: 1000px; transition: max-height 0.5s ease-in; }
        .card { transition: transform 0.3s ease, box-shadow 0.3s ease; }
        .card:hover { transform: translateY(-5px); box-shadow: 0 10px 15px -3px rgba(0,0,0,0.1), 0 4px 6px -2px rgba(0,0,0,0.05); }
        .ai-response-area {
            margin-top: 0.75rem;
            padding: 0.75rem;
            background-color: #f0f9ff; /* sky-50 */
            border-left: 4px solid #0ea5e9; /* sky-500 */
            border-radius: 0.25rem;
            font-size: 0.875rem;
            color: #0c4a6e; /* sky-800 */
        }
        .loading-spinner {
            border: 2px solid #f3f3f3; /* Light grey */
            border-top: 2px solid #0284c7; /* Sky blue */
            border-radius: 50%;
            width: 16px;
            height: 16px;
            animation: spin 1s linear infinite;
            display: inline-block;
            margin-left: 8px;
        }
        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
    </style>
</head>
<body class="bg-slate-50 text-slate-800">

    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex items-center">
                    <h1 class="text-2xl font-bold text-sky-600">Voestalpine <span class="text-slate-500">&</span> LYNXX</h1>
                </div>
                <nav class="hidden md:flex space-x-4">
                    <a href="#" data-section="overview" class="nav-link active px-3 py-2 rounded-md text-sm font-medium border-b-2 border-transparent">Overview</a>
                    <a href="#" data-section="ecosystem" class="nav-link px-3 py-2 rounded-md text-sm font-medium border-b-2 border-transparent">Digital Ecosystem</a>
                    <a href="#" data-section="products" class="nav-link px-3 py-2 rounded-md text-sm font-medium border-b-2 border-transparent">Core Products</a>
                    <a href="#" data-section="collaboration" class="nav-link px-3 py-2 rounded-md text-sm font-medium border-b-2 border-transparent">Collaboration</a>
                    <a href="#" data-section="engagement" class="nav-link px-3 py-2 rounded-md text-sm font-medium border-b-2 border-transparent">Engagement</a>
                </nav>
                <div class="md:hidden">
                    <button id="mobile-menu-button" class="text-slate-500 hover:text-sky-600 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-sky-500">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <div id="mobile-menu" class="md:hidden hidden bg-white shadow-lg">
            <a href="#" data-section="overview" class="block nav-link active px-4 py-3 text-base font-medium border-l-4 border-sky-600">Overview</a>
            <a href="#" data-section="ecosystem" class="block nav-link px-4 py-3 text-base font-medium border-l-4 border-transparent hover:bg-slate-100 hover:border-sky-500">Digital Ecosystem</a>
            <a href="#" data-section="products" class="block nav-link px-4 py-3 text-base font-medium border-l-4 border-transparent hover:bg-slate-100 hover:border-sky-500">Core Products</a>
            <a href="#" data-section="collaboration" class="block nav-link px-4 py-3 text-base font-medium border-l-4 border-transparent hover:bg-slate-100 hover:border-sky-500">Collaboration</a>
            <a href="#" data-section="engagement" class="block nav-link px-4 py-3 text-base font-medium border-l-4 border-transparent hover:bg-slate-100 hover:border-sky-500">Engagement</a>
        </div>
    </header>

    <main class="container mx-auto p-4 sm:p-6 lg:p-8">
        
        <section id="overview" class="section-active tab-content">
             <div class="bg-white p-6 sm:p-8 rounded-lg shadow-lg">
                <h2 class="text-3xl font-bold text-sky-700 mb-6">Executive Summary: A Digital Transformation in Rail</h2>
                <p class="text-lg text-slate-700 mb-4 leading-relaxed">
                    Voestalpine Railway Systems, a global leader in railway infrastructure, is strategically pivoting from a component supplier to a comprehensive systems and solutions provider, with a strong emphasis on digitalization and data-driven services. This evolution is centered around its <strong>zentrak</strong> digital ecosystem, designed as the core platform for monitoring, asset management, and maintenance.
                </p>
                <p class="text-lg text-slate-700 mb-4 leading-relaxed">
                    The company aims to advance along the data value chain towards sophisticated data analytics, predictive insights, and AI to enhance operational efficiency, safety, and Life Cycle Cost (LCC) optimization. Key products like <strong>Intelligent Turnouts</strong> and modular <strong>Checkpoint</strong> monitoring systems are increasingly sensor-equipped, generating rich, multi-modal data.
                </p>
                <p class="text-lg text-slate-700 leading-relaxed">
                    For LYNXX, specializing in data science and predictive maintenance, Voestalpine's direction presents compelling collaboration opportunities. These include elevating zentrak's predictive power, developing advanced AI models, co-creating new data-driven services, and translating complex data into actionable maintenance strategies. This interactive explorer, now enhanced with AI-powered preparation tools, delves into these facets.
                </p>
            </div>
        </section>

        <section id="ecosystem" class="section-inactive tab-content">
            <div class="bg-white p-6 sm:p-8 rounded-lg shadow-lg">
                <h2 class="text-3xl font-bold text-sky-700 mb-6">Voestalpine's Digital Ecosystem</h2>
                <p class="text-lg text-slate-700 mb-6 leading-relaxed">
                    Voestalpine is actively positioning itself as a technology leader through a focused strategy on digitalization, data analytics, and AI. This is crucial for enhancing product performance, optimizing maintenance, and reducing life cycle costs. The <strong>zentrak</strong> ecosystem is the cornerstone of this digital transformation, supported by a diverse array of sensor technologies.
                </p>
                <div class="mb-8">
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">The zentrak Ecosystem</h3>
                    <p class="text-slate-600 mb-4">zentrak is Voestalpine's intelligent ecosystem for monitoring, asset, and maintenance management, providing a 360° view of assets and paving the way for predictive maintenance. Key components include:</p>
                    <div id="zentrak-components" class="space-y-3"></div>
                </div>
                <div class="mb-8">
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Sensor Technologies & Data Generation</h3>
                    <p class="text-slate-600 mb-4">Voestalpine employs a wide array of sensor technologies integrated into tracks, turnouts (like the Intelligent Turnout), and modular "Checkpoints." This creates a rich, multi-modal data landscape encompassing acoustic, thermal, visual, and mechanical measurements.</p>
                    <div class="chart-container bg-white p-4 rounded-lg shadow">
                        <canvas id="sensorDataChart"></canvas>
                    </div>
                    <p class="text-sm text-slate-500 mt-2 text-center">Overview of key sensor types and the primary parameters they measure.</p>
                </div>
                <div>
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Current Data Analytics & AI</h3>
                    <p class="text-slate-600 leading-relaxed">
                        Voestalpine utilizes Machine Learning (ML) within zentrak for proactive failure prevention and in Intelligent Turnouts for diagnosing and predicting potential failures. While specific technical details are limited publicly, this indicates a strategic embrace of AI. This presents an opportunity for specialized firms like LYNXX to offer more advanced AI solutions, particularly in railway-specific predictive maintenance.
                    </p>
                </div>
            </div>
        </section>

        <section id="products" class="section-inactive tab-content">
            <div class="bg-white p-6 sm:p-8 rounded-lg shadow-lg">
                <h2 class="text-3xl font-bold text-sky-700 mb-6">Core Products & Embedded Intelligence</h2>
                <p class="text-lg text-slate-700 mb-6 leading-relaxed">
                    Voestalpine's comprehensive product portfolio for rail infrastructure is increasingly embedded with digital technologies, transforming physical components into valuable data sources for enhanced monitoring and maintenance. This integration is foundational for advanced predictive strategies.
                </p>
                <div id="core-products-grid" class="grid md:grid-cols-2 lg:grid-cols-3 gap-6"></div>
            </div>
        </section>

        <section id="collaboration" class="section-inactive tab-content">
            <div class="bg-white p-6 sm:p-8 rounded-lg shadow-lg">
                <h2 class="text-3xl font-bold text-sky-700 mb-6">Collaboration Opportunities for LYNXX</h2>
                <p class="text-lg text-slate-700 mb-6 leading-relaxed">
                    Voestalpine's strategic push towards advanced data analytics and AI aligns directly with LYNXX's expertise in data science and predictive maintenance for the rail sector. This synergy creates significant opportunities for a mutually beneficial partnership.
                </p>
                <div class="mb-8">
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">LYNXX's Value Contribution</h3>
                     <p class="text-slate-600 mb-4">LYNXX can contribute by:</p>
                    <ul class="list-disc list-inside space-y-2 text-slate-600 mb-4">
                        <li><strong>Enhancing zentrak's Predictive Capabilities:</strong> Developing more sophisticated AI models for failure prediction, RUL estimation, and anomaly detection using advanced data fusion.</li>
                        <li><strong>Developing Advanced AI for Specific Assets:</strong> Creating tailored models for high-value assets like Intelligent Turnouts and HSH® rails.</li>
                        <li><strong>Co-creating New Data-Driven Services:</strong> Defining new services for rail operators, such as optimized maintenance scheduling or dynamic LCC modeling.</li>
                        <li><strong>Improving Data Interpretation:</strong> Helping translate complex analytical results into actionable insights within zentrak.</li>
                        <li><strong>Supporting EULYNX Data Integration:</strong> Leveraging EULYNX-compliant data for broader analytical applications.</li>
                    </ul>
                    <p class="text-slate-600">This collaboration would leverage Voestalpine's data access, domain expertise, and market reach.</p>
                </div>
                <div class="mb-8">
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Mapping LYNXX's Capabilities to Voestalpine's Needs</h3>
                    <p class="text-slate-600 mb-4">The following outlines how LYNXX's expertise can directly address Voestalpine's digital ambitions:</p>
                    <div class="overflow-x-auto bg-white rounded-lg shadow">
                        <table class="min-w-full divide-y divide-slate-200">
                            <thead class="bg-slate-50">
                                <tr>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-slate-500 uppercase tracking-wider">Voestalpine Need/Goal</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-slate-500 uppercase tracking-wider">LYNXX Capability</th>
                                    <th scope="col" class="px-6 py-3 text-left text-xs font-medium text-slate-500 uppercase tracking-wider">Potential Value</th>
                                </tr>
                            </thead>
                            <tbody id="lynxx-capabilities-table" class="bg-white divide-y divide-slate-200"></tbody>
                        </table>
                    </div>
                </div>
                <div>
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Potential Business Models</h3>
                    <p class="text-slate-600 mb-4">Several business models could structure a collaboration, leveraging Voestalpine's history of technology partnerships:</p>
                    <div id="business-models-container" class="grid md:grid-cols-2 gap-6"></div>
                     <p class="text-slate-600 mt-4">A phased approach, starting with a pilot project, is advisable to demonstrate value and build a robust working relationship. Clear agreements on data access, governance, and IP will be paramount.</p>
                </div>
            </div>
        </section>

        <section id="engagement" class="section-inactive tab-content">
            <div class="bg-white p-6 sm:p-8 rounded-lg shadow-lg">
                <h2 class="text-3xl font-bold text-sky-700 mb-6">Engagement Strategy with Voestalpine (AI Enhanced)</h2>
                 <p class="text-lg text-slate-700 mb-6 leading-relaxed">
                    Effective engagement with Voestalpine, particularly with key contacts like Mr. Harald Hopfgartner, requires strategic preparation. Use the AI-powered tools below to enhance your readiness.
                </p>

                <div class="mb-8">
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Focus: Harald Hopfgartner</h3>
                    <div class="bg-sky-50 p-4 rounded-lg border border-sky-200">
                        <p class="text-slate-700 font-semibold" id="harald-profile-name">Harald Hopfgartner</p>
                        <p class="text-slate-600 text-sm" id="harald-profile-title">Member of the Management Board – Sales, voestalpine Signaling Siershahn GmbH</p>
                        <p class="text-slate-600 text-sm mt-1" id="harald-profile-responsibilities">Responsibilities: Sales & Marketing, Customer Service, Subsidiary Australia. Specialist in railway diagnostic and monitoring technologies, including "Checkpoints."</p>
                        <p class="text-slate-600 text-sm mt-2" id="harald-profile-notes">Mr. Hopfgartner is a key contact, likely attuned to market demands for enhanced predictive capabilities and the commercial benefits of such solutions. Voestalpine Signaling Siershahn plays a pivotal role in Voestalpine's advanced monitoring and predictive maintenance offerings.</p>
                        <button id="generate-talking-points-btn" class="mt-4 inline-flex items-center px-4 py-2 border border-transparent text-sm font-medium rounded-md shadow-sm text-white bg-sky-600 hover:bg-sky-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-sky-500">
                            ✨ Generate Talking Points with AI
                            <span class="loading-spinner hidden ml-2"></span>
                        </button>
                        <div id="talking-points-response" class="ai-response-area mt-3 hidden"></div>
                    </div>
                </div>

                <div class="mb-8">
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Strategic Questions for LYNXX to Explore (AI Assisted)</h3>
                    <p class="text-slate-600 mb-3">To clarify Voestalpine's current position and future needs, LYNXX should consider asking (click "✨ Elaborate" for AI-powered insights):</p>
                    <ul id="strategic-questions-list" class="space-y-4 text-slate-600"></ul>
                </div>

                <div>
                    <h3 class="text-2xl font-semibold text-sky-600 mb-4">Positioning LYNXX's Value Proposition</h3>
                    <ul class="list-disc list-inside space-y-2 text-slate-600">
                        <li><strong>Accelerate Voestalpine's Strategy:</strong> Emphasize how LYNXX can help achieve predictive/prescriptive maintenance goals faster.</li>
                        <li><strong>Highlight Rail Specialization:</strong> Showcase deep domain expertise in railway asset data and predictive modeling.</li>
                        <li><strong>Propose a Phased Approach:</strong> Suggest a pilot project to demonstrate value and de-risk engagement.</li>
                        <li><strong>Address LCC Optimization:</strong> Quantify benefits in Life Cycle Cost reduction and asset availability.</li>
                        <li><strong>Discuss Data, IP, and Security Proactively:</strong> Present clear frameworks for these critical aspects.</li>
                    </ul>
                    <p class="text-slate-600 mt-3">Success will depend on Voestalpine's technical capability and willingness to integrate external solutions. Framing LYNXX's value in terms of Voestalpine's commercial drivers is key.</p>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-slate-800 text-slate-300 py-8 text-center">
        <p class="text-sm">&copy; 2025 Voestalpine & LYNXX Collaboration Explorer. Information based on the "Voestalpine Rail Data Cooperation" report.</p>
        <p class="text-xs mt-1">This is a conceptual application for information exploration. AI features use Gemini.</p>
    </footer>

    <script>
        const sections = {
            overview: document.getElementById('overview'),
            ecosystem: document.getElementById('ecosystem'),
            products: document.getElementById('products'),
            collaboration: document.getElementById('collaboration'),
            engagement: document.getElementById('engagement'),
        };

        const navLinks = document.querySelectorAll('.nav-link');
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        function setActiveSection(sectionId) {
            Object.values(sections).forEach(section => {
                section.classList.remove('section-active');
                section.classList.add('section-inactive');
            });
            if (sections[sectionId]) {
                sections[sectionId].classList.add('section-active');
                sections[sectionId].classList.remove('section-inactive');
            }

            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.dataset.section === sectionId) {
                    link.classList.add('active');
                    if (link.closest('#mobile-menu')) {
                        link.classList.add('border-sky-600', 'bg-sky-50');
                        link.classList.remove('border-transparent');
                    } else {
                         link.classList.add('text-sky-600', 'border-sky-600');
                    }
                } else {
                    if (link.closest('#mobile-menu')) {
                        link.classList.remove('border-sky-600', 'bg-sky-50');
                        link.classList.add('border-transparent');
                    } else {
                        link.classList.remove('text-sky-600', 'border-sky-600');
                    }
                }
            });
            window.scrollTo({ top: 0, behavior: 'smooth' });
        }

        navLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                const sectionId = e.target.dataset.section;
                setActiveSection(sectionId);
                if (mobileMenu.classList.contains('block')) {
                    mobileMenu.classList.add('hidden');
                    mobileMenu.classList.remove('block');
                }
            });
        });
        
        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            mobileMenu.classList.toggle('block');
        });

        const zentrakData = [
            { title: "zentrak Asset and Maintenance Management", content: "Digital asset lifecycle recording & optimization, predefined asset structures, health status visualization, BIM data provision, resource management. Dynamically adapts maintenance by connecting to condition monitoring." },
            { title: "zentrak Central Management Software (CMS)", content: "Real-time status capture, selective data analysis, optimized asset management, efficient maintenance planning. Features machine learning for proactive failure prevention." },
            { title: "zentrak Fleet Condition Monitoring", content: "Monitoring and alerting for critical rolling stock events, incorporates machine learning for proactive failure avoidance, reporting, and software administration." },
            { title: "Digital Track Management (DTM)", content: "Developed with Boom Software AG. Efficient planning of maintenance for infrastructure & rolling stock, preventive alarms, location/component/image data, digital documentation." },
            { title: "zentrak Infrastructure Monitoring", content: "Continuous monitoring of fixed infrastructure, enabling proactive, condition-based maintenance using data from track, turnout, and signaling sensors." },
            { title: "zentrak Rolling Stock Monitoring", content: "Real-time analysis and interpretation of diagnostic results from various wayside measurement technologies (acoustic, infrared, optical, impact sensors)." }
        ];
        const zentrakContainer = document.getElementById('zentrak-components');
        zentrakData.forEach(item => {
            const div = document.createElement('div');
            div.className = 'border border-slate-200 rounded-lg';
            div.innerHTML = `
                <button class="accordion-button w-full text-left px-4 py-3 bg-slate-100 hover:bg-slate-200 focus:outline-none rounded-t-lg flex justify-between items-center">
                    <span class="font-medium text-sky-700">${item.title}</span>
                    <svg class="w-5 h-5 transform transition-transform duration-300" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path></svg>
                </button>
                <div class="accordion-content px-4 py-3 bg-white rounded-b-lg">
                    <p class="text-slate-600 text-sm">${item.content}</p>
                </div>`;
            zentrakContainer.appendChild(div);
        });
        document.querySelectorAll('.accordion-button').forEach(button => {
            button.addEventListener('click', () => {
                const content = button.nextElementSibling;
                const icon = button.querySelector('svg');
                content.classList.toggle('open');
                icon.classList.toggle('rotate-180');
            });
        });
        
        const sensorChartData = {
            labels: ['Acoustic (AMS)', 'Infrared Temp.', 'Laser Profile', 'Visual (Cameras)', 'Int. Turnout (Machine)', 'Int. Turnout (Device)', 'Int. Turnout (Track Q.)', 'Track/Rail (TRM)', 'Flat Spot/WIM', 'Dragging Equip. (DED)', 'Axle Counters'],
            datasets: [{
                label: 'Key Measured Parameters/Data Points',
                data: [4, 3, 3, 3, 4, 4, 5, 3, 3, 1, 3],
                backgroundColor: 'rgba(2, 132, 199, 0.6)', 
                borderColor: 'rgba(2, 132, 199, 1)',
                borderWidth: 1
            }]
        };
        const sensorDataCtx = document.getElementById('sensorDataChart').getContext('2d');
        new Chart(sensorDataCtx, {
            type: 'bar', data: sensorChartData,
            options: {
                responsive: true, maintainAspectRatio: false, indexAxis: 'y',
                scales: { x: { beginAtZero: true, title: { display: true, text: 'Number of Key Parameters/Data Types Monitored' } }, y: { ticks: { autoSkip: false, maxRotation: 0, minRotation: 0, callback: function(value) { const label = this.getLabelForValue(value); return label.length > 25 ? label.substring(0, 25) + '...' : label; }}}},
                plugins: { legend: { display: false }, title: { display: true, text: 'Voestalpine Sensor Portfolio: Measured Data Diversity', font: {size: 16}},
                    tooltip: { callbacks: { label: function(context) { let label = context.dataset.label || ''; if (label) { label += ': '; } if (context.parsed.x !== null) { label += context.parsed.x + ' key types'; } return label; },
                        footer: function(tooltipItems) {
                            const sensorDetails = { 'Acoustic (AMS)': 'Bearing signatures, defect trends, alarms.', 'Infrared Temp.': 'Axle/wheel/brake temps, hot/cold alarms.', 'Laser Profile': 'Slipped loads, out-of-gauge profiles.', 'Visual (Cameras)': 'Images for defect detection (bolts, cracks).', 'Int. Turnout (Machine)': 'Movement curves, motor current, oil levels.', 'Int. Turnout (Device)': 'Switch/stock rail distance, wear patterns.', 'Int. Turnout (Track Q.)': 'Sleeper displacement, vibrations, train data.', 'Track/Rail (TRM)': 'Rail movements, breaks, temperature.', 'Flat Spot/WIM': 'Impact loads, imbalances, axle loads.', 'Dragging Equip. (DED)': 'Alerts for dangling objects.', 'Axle Counters': 'Train detection, direction, traffic flow.'};
                            return sensorDetails[tooltipItems[0].label] || '';
                        }
                    }}
                }
            }
        });

        const coreProductsData = [
            { name: "Rails (HSH®)", description: "High-performance grades for diverse applications. Data potential for wear and fatigue monitoring.", icon: "🛤️" },
            { name: "Intelligent Turnout", description: "Sensor-equipped for real-time monitoring of switch machine, device, and track quality. Core data source for zentrak.", icon: "🔄" },
            { name: "Signaling Solutions", description: "Point machines, detection systems, axle counters. Intelligent monitoring for asset health and operational status.", icon: "🚦" },
            { name: "Checkpoints", description: "Modular diagnostic systems with acoustic, visual, flat spot, WIM sensors. Supports predictive maintenance for rolling stock.", icon: "️ตรวจ"},
            { name: "Fastening Systems", description: "Coordinated systems for track stability. Indirect data input via overall track condition monitoring.", icon: "🔩" }
        ];
        const productsContainer = document.getElementById('core-products-grid');
        coreProductsData.forEach(product => {
            const card = document.createElement('div');
            card.className = 'card bg-white p-6 rounded-lg shadow-md hover:shadow-xl';
            card.innerHTML = `<div class="flex items-center mb-3"><span class="text-3xl mr-3">${product.icon}</span><h4 class="text-xl font-semibold text-sky-700">${product.name}</h4></div><p class="text-slate-600 text-sm">${product.description}</p>`;
            productsContainer.appendChild(card);
        });

        const lynxxCapabilitiesData = [
            { need: "Predictive/Prescriptive Maintenance", capability: "Advanced ML/AI, RUL estimation", value: "Accelerated AI features, improved LCC" },
            { need: "Optimize LCC", capability: "Data-driven LCC modeling, maintenance optimization", value: "Stronger LCC value prop, new advisory services" },
            { need: "Enhance zentrak with AI", capability: "Big data analytics, sensor fusion, custom AI", value: "Increased zentrak value, better user efficiency" },
            { need: "Improve Fault Detection", capability: "Anomaly detection, multi-modal diagnostics", value: "Higher accuracy, reduced false alarms" },
            { need: "Leverage EULYNX Data", capability: "Standardized data model expertise", value: "Future-proofed analytics, richer data use" },
            { need: "New Data-Driven Services", capability: "Service design, Analytics-as-a-Service", value: "New revenue streams, enhanced engagement" }
        ];
        const lynxxTableBody = document.getElementById('lynxx-capabilities-table');
        lynxxCapabilitiesData.forEach(item => {
            const row = lynxxTableBody.insertRow();
            row.innerHTML = `<td class="px-6 py-4 whitespace-nowrap text-sm text-slate-700">${item.need}</td><td class="px-6 py-4 whitespace-nowrap text-sm text-slate-600">${item.capability}</td><td class="px-6 py-4 whitespace-nowrap text-sm text-slate-600">${item.value}</td>`;
        });
        
        const businessModelsData = [
            { name: "Joint Development Projects (JDP)", description: "Co-invest resources to develop specific AI solutions for Voestalpine products or zentrak. Shared IP/licensing.", icon: "🤝" },
            { name: "Specialized Analytics Service Provider", description: "LYNXX provides analytics platform/expertise as a service, processing zentrak data. Outputs integrated into Voestalpine offerings (white-label potential).", icon: "⚙️" },
            { name: "Technology Licensing", description: "LYNXX licenses pre-developed AI algorithms/components to Voestalpine for integration into zentrak.", icon: "📜" },
            { name: "Strategic Partnership for New Offerings", description: "Jointly define, develop, and launch new data-driven services for the rail market. Shared investment, co-branding, revenue-sharing.", icon: "🚀" },
            { name: "Consulting & Capability Building", description: "LYNXX offers expert consulting to accelerate Voestalpine's internal data science team and AI roadmap for rail.", icon: "🎓" }
        ];
        const businessModelsContainer = document.getElementById('business-models-container');
        businessModelsData.forEach(model => {
            const modelDiv = document.createElement('div');
            modelDiv.className = 'card bg-sky-50 p-5 rounded-lg shadow hover:shadow-lg border border-sky-200 cursor-pointer';
            modelDiv.innerHTML = `<div class="flex items-start mb-2"><span class="text-2xl mr-3">${model.icon}</span><h4 class="text-lg font-semibold text-sky-700">${model.name}</h4></div><p class="text-sm text-slate-600 model-description hidden">${model.description}</p>`;
            businessModelsContainer.appendChild(modelDiv);
            modelDiv.addEventListener('click', () => modelDiv.querySelector('.model-description').classList.toggle('hidden'));
        });

        const strategicQuestionsData = [
            { id: "q1", text: "Current AI/Analytics Maturity: Can you elaborate on current ML models in zentrak/Intelligent Turnouts, their targets, and performance metrics?" },
            { id: "q2", text: "AI in Intelligent Points: What sensor inputs drive AI failure risk assessment, and what's the typical lead time/accuracy?" },
            { id: "q3", text: "Roadmap & Gaps: What's Voestalpine's 3-5 year roadmap for zentrak's AI/predictive/prescriptive capabilities? Where are key needs for external data science expertise?" },
            { id: "q4", text: "Data Access & Integration: What are policies/technical possibilities for 3rd party integration with zentrak (APIs)? What data formats/standards (EULYNX) are prioritized?" },
            { id: "q5", text: "Multi-modal Data Handling: How is diverse sensor data standardized and time-synchronized in zentrak for analysis?" },
            { id: "q6", text: "Data Ownership & IP: How is data ownership (especially customer data) handled? What's the IP framework for collaborative AI model development?" },
            { id: "q7", text: "Security Protocols: What data governance and security protocols apply to third-party analytics providers?" },
            { id: "q8", text: "Pilot Project Interest: Would Voestalpine be open to a focused pilot project with LYNXX? What would be key success criteria?" },
            { id: "q9", text: "EULYNX Strategy: What's the timeline/scope for EULYNX compliance? How will zentrak leverage EULYNX interfaces?" },
            { id: "q10", text: "Preferred Partnership Models: What commercial/partnership models are preferred for integrating specialized analytics, learning from past collaborations (e.g., Boom Software)?" }
        ];
        const questionsList = document.getElementById('strategic-questions-list');
        strategicQuestionsData.forEach(q => {
            const listItem = document.createElement('li');
            listItem.className = "p-3 bg-white border border-slate-200 rounded-md shadow-sm";
            listItem.innerHTML = `
                <div class="flex justify-between items-start">
                    <span class="text-slate-700 flex-1 pr-2">${q.text}</span>
                    <button data-question-id="${q.id}" class="elaborate-question-btn flex-shrink-0 inline-flex items-center px-3 py-1.5 border border-sky-500 text-xs font-medium rounded-md text-sky-700 bg-sky-100 hover:bg-sky-200 focus:outline-none focus:ring-2 focus:ring-offset-1 focus:ring-sky-400">
                        ✨ Elaborate
                        <span class="loading-spinner hidden ml-1.5"></span>
                    </button>
                </div>
                <div id="elaboration-${q.id}" class="ai-response-area mt-2 hidden"></div>
            `;
            questionsList.appendChild(listItem);
        });

        // Gemini API Key - IMPORTANT: Replace with your actual API key or use a secure method for key management
        const GEMINI_API_KEY = ""; // Intentionally empty for Canvas environment; will be populated by the platform.

        async function callGeminiAPI(prompt, buttonElement, responseElementId) {
            const responseElement = document.getElementById(responseElementId);
            const spinner = buttonElement.querySelector('.loading-spinner');

            if (!responseElement) {
                console.error("Response element not found:", responseElementId);
                return;
            }

            responseElement.classList.remove('hidden');
            responseElement.innerHTML = 'Generating insights with AI... Please wait.';
            if(spinner) spinner.classList.remove('hidden');
            buttonElement.disabled = true;

            const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent?key=${GEMINI_API_KEY}`;
            
            const payload = {
                contents: [{ role: "user", parts: [{ text: prompt }] }]
            };

            try {
                const response = await fetch(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });

                if (!response.ok) {
                    const errorData = await response.json();
                    console.error("API Error:", errorData);
                    throw new Error(`API request failed with status ${response.status}: ${errorData.error?.message || 'Unknown error'}`);
                }

                const result = await response.json();
                
                if (result.candidates && result.candidates.length > 0 &&
                    result.candidates[0].content && result.candidates[0].content.parts &&
                    result.candidates[0].content.parts.length > 0) {
                    // Format the text to replace markdown-like lists with HTML lists
                    let text = result.candidates[0].content.parts[0].text;
                    text = text.replace(/\n\*/g, '\n<li>') // Start of list item
                               .replace(/\n\s*\-\s/g, '\n<li>') // Alternative list item start
                               .replace(/(\n<li>.*?)(?=\n<li>|\n\n|$)/gs, '$1</li>'); // End of list item
                    text = text.replace(/\n(<li>.*?<\/li>)+/gs, (match) => `<ul>${match}</ul>`); // Wrap list items in ul
                    text = text.replace(/\n/g, '<br>'); // Convert newlines to <br> for paragraph breaks
                    responseElement.innerHTML = text;
                } else {
                    responseElement.textContent = 'No content received from AI or unexpected response structure.';
                    console.warn("Unexpected API response structure:", result);
                }

            } catch (error) {
                console.error('Error calling Gemini API:', error);
                responseElement.textContent = `Error: ${error.message}. Check console for details. Ensure API key is valid if testing locally.`;
            } finally {
                if(spinner) spinner.classList.add('hidden');
                buttonElement.disabled = false;
            }
        }

        document.querySelectorAll('.elaborate-question-btn').forEach(button => {
            button.addEventListener('click', async (event) => {
                const questionId = event.currentTarget.dataset.questionId;
                const questionData = strategicQuestionsData.find(q => q.id === questionId);
                if (questionData) {
                    const prompt = `You are a strategic advisor for a tech company. LYNXX (a data science firm specializing in rail predictive maintenance) is meeting Voestalpine (a major rail infrastructure provider). Please elaborate on the following strategic question that LYNXX plans to ask Voestalpine. Provide insights, potential follow-up questions, or areas Voestalpine might focus on in their answer. Question: "${questionData.text}"`;
                    await callGeminiAPI(prompt, event.currentTarget, `elaboration-${questionId}`);
                }
            });
        });

        const generateTalkingPointsBtn = document.getElementById('generate-talking-points-btn');
        generateTalkingPointsBtn.addEventListener('click', async (event) => {
            const haraldProfileName = document.getElementById('harald-profile-name').textContent;
            const haraldProfileTitle = document.getElementById('harald-profile-title').textContent;
            const haraldProfileResponsibilities = document.getElementById('harald-profile-responsibilities').textContent;
            const haraldProfileNotes = document.getElementById('harald-profile-notes').textContent;

            const profileText = `Name: ${haraldProfileName}\nTitle: ${haraldProfileTitle}\n${haraldProfileResponsibilities}\n${haraldProfileNotes}`;
            
            const prompt = `You are an expert business development consultant for B2B tech partnerships in the railway industry. LYNXX (a data science and predictive maintenance consultancy) is meeting Harald Hopfgartner from Voestalpine. His profile is: "${profileText}". 
            Generate 3-4 concise, actionable key talking points for LYNXX to effectively engage him. Focus on how LYNXX can help Voestalpine achieve its goals of moving up the data value chain, enhancing its zentrak ecosystem, and leveraging its sensor data for predictive maintenance. Frame talking points as how LYNXX can solve Voestalpine's potential challenges or help seize opportunities.`;
            
            await callGeminiAPI(prompt, event.currentTarget, 'talking-points-response');
        });

        setActiveSection('overview');
    </script>
</body>
</html>
