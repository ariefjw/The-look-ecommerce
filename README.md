# 📊 E-commerce Operational Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/downloads/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-success.svg)]()

## 📋 Table of Contents
- [Overview](#overview)
- [Project Status](#project-status)
- [Problem Statement](#problem-statement)
- [Data Sources](#data-sources)
- [Key Findings](#key-findings)
- [Visualizations](#visualizations)
- [Technical Requirements](#technical-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Troubleshooting](#troubleshooting)
- [Analysis Structure](#analysis-structure)
- [Contributing](#contributing)
- [Contact](#contact)
- [License](#license)

## 🔍 Overview
This project presents a comprehensive analysis of an e-commerce company's operational performance, focusing on inventory management and shipping efficiency. The analysis aims to identify key challenges and opportunities for improvement in the company's operations, providing actionable insights for business optimization.

## 📈 Project Status
- ✅ Data Collection: Complete
- ✅ Data Cleaning: Complete
- ✅ Analysis: Complete
- ✅ Visualization: Complete
- ✅ Documentation: In Progress
- 🔄 Future Updates: Planned

## 🎯 Problem Statement
The e-commerce company faces several operational challenges that impact efficiency and customer satisfaction. This analysis addresses two main areas:

### 🚚 Shipping Performance
- Variation in delivery duration across different regions
- Analysis of order cancellations and returns
- Distribution efficiency optimization
- Shipping time optimization
- Regional performance analysis

### 📦 Inventory Management
- Significant variation in stock age across product categories
- Low stock turnover in certain categories
- Safety stock optimization
- Overstocking indicators in specific categories
- Seasonal demand patterns

## 📊 Data Sources
The analysis utilizes the following datasets:

| Dataset | Description | Size | Update Frequency |
|---------|-------------|------|------------------|
| `inventory_items.csv` | Inventory tracking data | ~10MB | Daily |
| `order.csv` | Order information | ~15MB | Real-time |
| `order_items.csv` | Detailed order items data | ~20MB | Real-time |
| `products.csv` | Product catalog | ~5MB | Weekly |
| `user.csv` | Customer information | ~8MB | Daily |
| `dc.csv` | Distribution center locations | ~1MB | Monthly |

## 📈 Key Findings

### Shipping Performance Metrics
| Metric | Value | Target | Status |
|--------|-------|--------|--------|
| Total Orders Processed | 11,272 | - | ✅ |
| Shipping Success Rate | 65.68% | >70% | ⚠️ |
| Average Shipping Time | 0.99 days | <1 day | ✅ |
| Average Delivery Time | 1.97 days | <2 days | ✅ |
| Late Shipping Rate (>1 day) | 33.05% | <20% | ⚠️ |

### Order Status Distribution
| Status | Count | Percentage | Trend |
|--------|-------|------------|-------|
| Shipped | 3,439 | 30.5% | ↗️ |
| Complete | 2,869 | 25.5% | ↗️ |
| Processing | 2,227 | 19.8% | → |
| Cancelled | 1,642 | 14.6% | ↘️ |
| Returned | 1,095 | 9.7% | → |

## 📊 Visualizations
The analysis includes several key visualizations:
- Shipping time distribution across regions
- Inventory turnover by product category
- Order status trends over time
- Regional performance heatmaps
- Product category performance analysis

## 💻 Technical Requirements
The analysis is performed using Python with the following key libraries:

```python
pandas>=1.3.0
numpy>=1.20.0
matplotlib>=3.4.0
seaborn>=0.11.0
scipy>=1.7.0
geopy>=2.2.0
jupyter>=1.0.0
```

## 🛠️ Installation

1. Clone the repository:
```bash
git clone [repository-url]
cd [repository-name]
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## 📝 Usage

1. Ensure all required Python packages are installed
2. Place all data files in the `Data` directory
3. Open the Jupyter notebook:
```bash
jupyter notebook analisa.ipynb
```
4. Run the notebook cells in sequence

## 🔧 Troubleshooting

### Common Issues
1. **Data Loading Errors**
   - Ensure all CSV files are in the correct directory
   - Check file permissions
   - Verify CSV file encoding (UTF-8)

2. **Package Installation Issues**
   - Update pip: `python -m pip install --upgrade pip`
   - Clear pip cache: `pip cache purge`
   - Try installing packages individually

3. **Memory Issues**
   - Use `pd.read_csv()` with `chunksize` parameter
   - Clear memory: `import gc; gc.collect()`

## 📑 Analysis Structure
1. Problem Statement
2. Data Loading and Preparation
3. Shipping Performance Analysis
4. Inventory Management Analysis
5. Recommendations and Conclusions

## 🤝 Contributing
We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

### Code Style
- Follow PEP 8 guidelines
- Use meaningful variable names
- Add comments for complex logic
- Include docstrings for functions

## 📧 Contact
For questions or suggestions, please contact:
- Email: ariefjkwicakson@gmail.com
- LinkedIn: [Arief Joko Wicasksono](https://www.linkedin.com/in/arief-joko-wicaksono-80a519141)
- GitHub Issues: [ariefjw](https://github.com/ariefjw)


---

<div align="center">
  <sub>Built by Arief Joko Wicaksono</sub>
</div> 