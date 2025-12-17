# Exchange rate monitor
#### by Jason Cao
### Overall:
A toy project, personal-use exchange monitor mainly for CNY to[EUR, USD, HKD, GBP, JPY] and exchange rates of 2 banks (BOC, CMB) in China.

这是一个实时监控外汇汇率（如 EUR/CNY, USD/CNY）的工具，支持桌面端和网页端。
数据来源：Yahoo Finance API (实时/历史) + 银行官网 (中国银行/招商银行)。

## 功能特点
- **多货币支持**：欧元、美元、港币、英镑、日元。
- **多时间周期**：1小时、24小时、48小时、7天、1个月、6个月、1年。
- **实时更新**：秒级刷新，实时显示涨跌幅。
- **交互式图表**：支持鼠标悬停查看具体数值，支持缩放。
- **双模式**：
  - 🖥️ **桌面版 (main.py)**: 基于 Matplotlib，适合本地长期挂机。
  - 🌐 **网页版 (app.py)**: 基于 Streamlit，适合部署或远程访问。

## 如何运行
### 0. (可选) 创建并激活虚拟环境
```bash
# 创建虚拟环境
python -m venv .venv

# 激活虚拟环境 (Windows PowerShell)
.\.venv\Scripts\Activate.ps1
```

### 1. 安装依赖
确保你安装了 Python 3.8+，然后运行：
```bash
pip install -r requirements.txt
```
### 2. 运行桌面版
```bash
python main.py
```
### 3. 运行网页版
```bash
streamlit run app.py
```