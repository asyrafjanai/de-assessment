# Credit Card Transaction Fraud Analysis (assessment)

## Project Overview
This project analyzes credit card transaction data with fraudulent cases using data processing, visualization, and distributed computing. The workflow involves data processing in Jupyter Notebook, data visualization with Power BI, and distributed data handling using Apache Spark in a Docker environment.

---

## Project Structure
```
├── work
│   └── data_processing.ipynb
├── cc_analysis.pdf
├── compose.yml
└── README.md
```

---

## Components

### 1. Dockerized Spark Setup
**Location:** `compose.yml`
- A Docker Compose configuration to spin up an Apache Spark cluster locally.
- Enables distributed data processing to handle large transaction datasets.
- Before running jupyter notebook, run the compose file to use spark as backend

**Services Included:**
- Spark Master Node
- Spark Worker Nodes
- JupyterLab for Spark interaction

**Run Docker Setup:**
```bash
cd docker
docker-compose up -d
```

**Access Spark UI:**
- Spark Master: [http://localhost:8080](http://localhost:8080)
- JupyterLab: [http://localhost:8888](http://localhost:8888)

---

### 2. Data Processing
**Location:** `work/data_processing.ipynb`
- A Jupyter Notebook that processes the credit card transaction data using pyspark
- Cleans data, detects patterns, and prepares the dataset for visualization.
- Outputs structured datasets ready for visualization and analysis.

**Requirements:**
- Python 3.8+
- Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn, PySpark (for distributed processing)


### 3. Data Visualization
**Location:** `cc_analysis.pdf`
- PDF report generated using Power BI.
- Contains visual insights such as fraud patterns, geographical distributions, and customer behavior analytics.

**Note:**
- Power BI file (.pbix) can be shared upon request for further edits or interaction.




## Getting Started
### Prerequisites
- Docker
- Power BI (for visualization edits)
- Jupyter Notebook

### Installation
1. Clone the repository:
```bash
git clone <repo-url>
```
2. Start the Spark cluster:
```bash
cd docker
docker-compose up -d
```
3. Open Jupyter Notebook and run `data_processing.ipynb`.
4. Review visualizations in `cc_analysis.pdf`.

---

## Data Sources
- [Kaggle dataset](https://www.kaggle.com/datasets/e47f88e5e8ce59c9598475a107d9a80ebc363a83859a59facb069b13a9001773)

---

## Contribution
Feel free to submit pull requests for improvements or reach out for collaboration.

---


## Contact
- **Email:** asyrafjanai[at]gmail.com
- **LinkedIn:** https://www.linkedin.com/in/asyrafjanai/

