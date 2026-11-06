# Machine Learning Coursework 2

Predictive modeling on the **Default of Credit Card Clients** dataset.

---

## Running with Docker (No Local Python/Virtual Environment Setup Required)

Anyone with [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed can run the entire notebook and environment with a single command.

### 1. Start the Environment

Open a terminal in this project directory and run:

```bash
docker compose up
```

*(Or without compose: `docker build -t ml-cw2 .` then `docker run -p 8888:8888 -v "%cd%":/app ml-cw2`)*

### 2. Open Jupyter in Browser

Open your browser and navigate to:

```
http://localhost:8888
```

All libraries (`pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`, `jupyter`) are pre-installed. Any changes you make or CSV files generated will automatically sync to your host computer.

### 3. Stop the Container

When finished, press `Ctrl + C` in the terminal, or run:

```bash
docker compose down
```

---

## Running Locally (Alternative)

If you prefer using a local Python virtual environment:

```bash
# 1. Create and activate virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1    # On Windows PowerShell

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch notebook
jupyter notebook
```
