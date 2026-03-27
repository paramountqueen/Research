# Research
Reasearch web<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Research Portal</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            padding: 20px;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 10px;
            box-shadow: 0 10px 40px rgba(0, 0, 0, 0.2);
            overflow: hidden;
        }

        header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 40px 20px;
            text-align: center;
        }

        header h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        header p {
            font-size: 1.1em;
            opacity: 0.9;
        }

        nav {
            background: #f8f9fa;
            padding: 0;
            display: flex;
            flex-wrap: wrap;
            border-bottom: 2px solid #e9ecef;
        }

        nav a {
            flex: 1;
            padding: 15px;
            text-align: center;
            text-decoration: none;
            color: #667eea;
            font-weight: 600;
            transition: all 0.3s ease;
            border-right: 1px solid #e9ecef;
        }

        nav a:last-child {
            border-right: none;
        }

        nav a:hover {
            background: #e9ecef;
            color: #764ba2;
        }

        .content {
            padding: 40px;
        }

        section {
            margin-bottom: 40px;
        }

        section h2 {
            color: #667eea;
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid #667eea;
        }

        .research-card {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 20px;
            border-left: 4px solid #667eea;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .research-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 20px rgba(102, 126, 234, 0.2);
        }

        .research-card h3 {
            color: #764ba2;
            margin-bottom: 10px;
        }

        .research-card p {
            color: #666;
            margin-bottom: 10px;
        }

        .tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 10px;
        }

        .tag {
            background: #667eea;
            color: white;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9em;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }

        table thead {
            background: #667eea;
            color: white;
        }

        table th, table td {
            padding: 12px;
            text-align: left;
        }

        table tbody tr {
            border-bottom: 1px solid #e9ecef;
        }

        table tbody tr:hover {
            background: #f8f9fa;
        }

        .search-box {
            margin-bottom: 30px;
        }

        .search-box input {
            width: 100%;
            padding: 12px;
            border: 2px solid #e9ecef;
            border-radius: 8px;
            font-size: 1em;
            transition: border-color 0.3s ease;
        }

        .search-box input:focus {
            outline: none;
            border-color: #667eea;
        }

        .filters {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }

        .filters button {
            padding: 10px 20px;
            border: 2px solid #667eea;
            background: white;
            color: #667eea;
            border-radius: 5px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
        }

        .filters button:hover,
        .filters button.active {
            background: #667eea;
            color: white;
        }

        .chart-container {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 8px;
            margin: 20px 0;
            text-align: center;
            min-height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #999;
        }

        footer {
            background: #f8f9fa;
            padding: 20px;
            text-align: center;
            color: #666;
            border-top: 1px solid #e9ecef;
        }

        .btn {
            display: inline-block;
            padding: 10px 20px;
            background: #667eea;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1em;
        }

        .btn:hover {
            background: #764ba2;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.8em;
            }

            nav {
                flex-direction: column;
            }

            nav a {
                border-right: none;
                border-bottom: 1px solid #e9ecef;
            }

            nav a:last-child {
                border-bottom: none;
            }

            .content {
                padding: 20px;
            }

            table {
                font-size: 0.9em;
            }

            table th, table td {
                padding: 8px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>🔬 Research Portal</h1>
            <p>Comprehensive Research Management & Analysis Platform</p>
        </header>

        <nav>
            <a href="#overview">Overview</a>
            <a href="#research">Research Papers</a>
            <a href="#data">Data & Statistics</a>
            <a href="#findings">Key Findings</a>
            <a href="#resources">Resources</a>
        </nav>

        <div class="content">
            <!-- Search Section -->
            <section>
                <h2>🔍 Search & Filter</h2>
                <div class="search-box">
                    <input type="text" placeholder="Search research papers, data, or keywords..." id="searchInput">
                </div>
                <div class="filters">
                    <button class="active">All</button>
                    <button>Recent</button>
                    <button>Popular</button>
                    <button>By Category</button>
                </div>
            </section>

            <!-- Overview Section -->
            <section id="overview">
                <h2>📊 Research Overview</h2>
                <div class="research-card">
                    <h3>Current Research Status</h3>
                    <p>This research portal provides comprehensive access to ongoing studies, data analysis, and research findings.</p>
                    <div class="tags">
                        <span class="tag">Active Study</span>
                        <span class="tag">Peer Reviewed</span>
                        <span class="tag">Data Available</span>
                    </div>
                </div>
            </section>

            <!-- Research Papers Section -->
            <section id="research">
                <h2>📚 Research Papers</h2>
                
                <div class="research-card">
                    <h3>Paper Title: Advanced Research Methodology</h3>
                    <p><strong>Authors:</strong> Dr. Smith, Dr. Johnson</p>
                    <p><strong>Published:</strong> March 2026</p>
                    <p>A comprehensive study examining modern research approaches and methodologies in contemporary science.</p>
                    <div class="tags">
                        <span class="tag">Methodology</span>
                        <span class="tag">Science</span>
                        <span class="tag">2026</span>
                    </div>
                    <button class="btn" style="margin-top: 10px;">Read Paper</button>
                </div>

                <div class="research-card">
                    <h3>Paper Title: Data Analysis Trends</h3>
                    <p><strong>Authors:</strong> Dr. Williams, Dr. Brown</p>
                    <p><strong>Published:</strong> February 2026</p>
                    <p>Analysis of current trends in data science and machine learning applications across various industries.</p>
                    <div class="tags">
                        <span class="tag">Data Science</span>
                        <span class="tag">Machine Learning</span>
                        <span class="tag">2026</span>
                    </div>
                    <button class="btn" style="margin-top: 10px;">Read Paper</button>
                </div>
            </section>

            <!-- Data & Statistics Section -->
            <section id="data">
                <h2>📈 Data & Statistics</h2>
                
                <div class="chart-container">
                    <p>📊 Charts and visualizations will be displayed here</p>
                </div>

                <table>
                    <thead>
                        <tr>
                            <th>Category</th>
                            <th>Sample Size</th>
                            <th>Success Rate</th>
                            <th>Status</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td>Study A</td>
                            <td>500 participants</td>
                            <td>94.5%</td>
                            <td>✅ Complete</td>
                        </tr>
                        <tr>
                            <td>Study B</td>
                            <td>750 participants</td>
                            <td>91.2%</td>
                            <td>✅ Complete</td>
                        </tr>
                        <tr>
                            <td>Study C</td>
                            <td>320 participants</td>
                            <td>88.7%</td>
                            <td>🔄 In Progress</td>
                        </tr>
                        <tr>
                            <td>Study D</td>
                            <td>600 participants</td>
                            <td>N/A</td>
                            <td>⏳ Pending</td>
                        </tr>
                    </tbody>
                </table>
            </section>

            <!-- Key Findings Section -->
            <section id="findings">
                <h2>🎯 Key Findings</h2>
                
                <div class="research-card">
                    <h3>Finding #1: Significant Correlation</h3>
                    <p>Our analysis revealed a statistically significant correlation between variables X and Y (p &lt; 0.05), suggesting a strong relationship in the data.</p>
                </div>

                <div class="research-card">
                    <h3>Finding #2: Improved Performance Metrics</h3>
                    <p>Implementation of new methodology resulted in a 23% improvement in overall performance metrics compared to baseline measurements.</p>
                </div>

                <div class="research-card">
                    <h3>Finding #3: Novel Insights</h3>
                    <p>The research identified three previously undocumented patterns in the data that warrant further investigation in future studies.</p>
                </div>
            </section>

            <!-- Resources Section -->
            <section id="resources">
                <h2>📚 Resources & References</h2>
                
                <div class="research-card">
                    <h3>Reference Materials</h3>
                    <ul style="margin-left: 20px; margin-top: 10px;">
                        <li><a href="#" style="color: #667eea;">Link to Dataset #1</a></li>
                        <li><a href="#" style="color: #667eea;">Link to Dataset #2</a></li>
                        <li><a href="#" style="color: #667eea;">Research Methodology Guide</a></li>
                        <li><a href="#" style="color: #667eea;">Statistical Analysis Tools</a></li>
                    </ul>
                </div>
            </section>
        </div>

        <footer>
            <p>&copy; 2026 Research Portal. All rights reserved. | <a href="#" style="color: #667eea;">Contact</a> | <a href="#" style="color: #667eea;">Privacy Policy</a></p>
        </footer>
    </div>

    <script>
        // Simple search functionality
        document.getElementById('searchInput').addEventListener('keyup', function(e) {
            const searchTerm = e.target.value.toLowerCase();
            const cards = document.querySelectorAll('.research-card');
            
            cards.forEach(card => {
                const text = card.textContent.toLowerCase();
                card.style.display = text.includes(searchTerm) ? 'block' : 'none';
            });
        });

        // Filter button functionality
        document.querySelectorAll('.filters button').forEach(button => {
            button.addEventListener('click', function() {
                document.querySelectorAll('.filters button').forEach(b => b.classList.remove('active'));
                this.classList.add('active');
            });
        });
    </script>
</body>
</html>
