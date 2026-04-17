# Exchange Rate Monitor
#### by Jason Cao

## English

### Overview
A toy project and personal-use exchange-rate monitor, mainly for CNY against EUR, USD, HKD, GBP, and JPY, plus exchange rates from two Chinese banks (BOC, CMB).

This is a real-time foreign exchange monitoring tool (such as EUR/CNY and USD/CNY), supporting both desktop and web interfaces.  
Data sources: Yahoo Finance API (real-time/historical) + bank official websites (Bank of China / China Merchants Bank).

### Features
- **Multi-currency support**: EUR, USD, HKD, GBP, JPY.
- **Multiple time ranges**: 1 hour, 24 hours, 48 hours, 7 days, 1 month, 6 months, 1 year.
- **Real-time updates**: second-level refresh with live percentage changes.
- **Interactive charts**: hover for exact values and zoom support.
- **Dual modes**:
  - 🖥️ **Desktop (main.py)**: based on Matplotlib, suitable for long-running local monitoring.
  - 🌐 **Web (app.py)**: based on Streamlit, suitable for deployment or remote access.

### How to Run
#### 0. (Optional) Create and activate a virtual environment
```bash
# Create virtual environment
python -m venv .venv

# Activate virtual environment (Windows PowerShell)
.\.venv\Scripts\Activate.ps1
```

#### 1. Install dependencies
Make sure Python 3.8+ is installed, then run:
```bash
pip install -r requirements.txt
```

#### 2. Run desktop app
```bash
python main.py
```

#### 3. Run web app
```bash
streamlit run app.py
```

## 中文

### 项目简介
这是一个实时监控外汇汇率（如 EUR/CNY、USD/CNY）的工具，支持桌面端和网页端。  
主要用于监控 CNY 对 EUR、USD、HKD、GBP、JPY 的汇率，以及中国银行、招商银行两家银行的汇率数据。  
数据来源：Yahoo Finance API（实时/历史）+ 银行官网（中国银行/招商银行）。

### 功能特点
- **多货币支持**：欧元、美元、港币、英镑、日元。
- **多时间周期**：1小时、24小时、48小时、7天、1个月、6个月、1年。
- **实时更新**：秒级刷新，实时显示涨跌幅。
- **交互式图表**：支持鼠标悬停查看具体数值，支持缩放。
- **双模式**：
  - 🖥️ **桌面版 (main.py)**：基于 Matplotlib，适合本地长期挂机。
  - 🌐 **网页版 (app.py)**：基于 Streamlit，适合部署或远程访问。

### 如何运行
#### 0. （可选）创建并激活虚拟环境
```bash
# 创建虚拟环境
python -m venv .venv

# 激活虚拟环境 (Windows PowerShell)
.\.venv\Scripts\Activate.ps1
```

#### 1. 安装依赖
确保你安装了 Python 3.8+，然后运行：
```bash
pip install -r requirements.txt
```

#### 2. 运行桌面版
```bash
python main.py
```

#### 3. 运行网页版
```bash
streamlit run app.py
```
