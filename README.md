# 📊 Mutual Fund Calculator & Planning Toolkit

An interactive personal finance and investment planning web app built with **Python**, **Streamlit**, and **Plotly**. It combines **SIP** and **Lumpsum** wealth calculators (with optional 6% inflation adjustment), **Time Value of Money (FV/PV)** utilities, Indian Rupee (`₹`) locale formatting, and an in-app mutual fund selection guide.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-App-FF4B4B?logo=streamlit&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-3F4F75?logo=plotly&logoColor=white)
![Babel](https://img.shields.io/badge/Babel-INR%20Locale%20Formatting-yellow)

---

## 📌 Overview

Retail investors often underestimate two forces in long-term financial planning: **compounding** and **inflation**. **Mutual Fund Calculator** brings four essential planning workflows into a single tabbed dashboard:

1. **SIP Calculator:** Project long-term wealth creation from monthly investments, with a one-click toggle to view inflation-adjusted real returns.
2. **Lumpsum Calculator:** Estimate compounded growth (CAGR) for one-time investments with real-return adjustments.
3. **Quick Tools (FV / PV):** Calculate the inflation-adjusted future cost of financial goals or discount future values back to today's purchasing power.
4. **MF Guide:** A beginner-friendly framework covering compounding, goal-based planning, and avoiding high-cost or overly complex fund categories.

---

## ✨ Key Features

- **SIP & Lumpsum Calculators:** Interactive sliders and numeric inputs for investment amount, expected annual return (`1%–30%`), and investment horizon.
- **Inflation Adjustment Toggle:** Dynamically recalculates projected corpus and net gain assuming a `6%` annual inflation rate to show real purchasing power.
- **Indian Currency Formatting:** Uses `babel.numbers` (`en_IN` locale) to format all outputs in standard Indian numbering format (lakhs/crores in `₹`).
- **Interactive Wealth Breakdown:** Renders Plotly pie charts comparing **Principal Invested** vs. **Estimated Wealth Gain** in real time.
- **Time Value of Money Utilities:** Side-by-side **Future Value (FV)** and **Present Value (PV)** calculators for goal sizing (e.g., retirement expenses, education costs).
- **Built-In Investor Education:** Structured 3-rule guide illustrating compounding and inflation through real-world INR scenarios.

---

## 🛠️ Tech Stack

| Component | Technology |
| :--- | :--- |
| **Language** | Python |
| **Frontend / UI** | Streamlit |
| **Visualizations** | Plotly (`plotly.graph_objects`) |
| **Localization / Currency** | Babel (`babel.numbers`) |
| **Data Handling** | Pandas |

---

## ⚙️ Core Formulas

- **SIP Future Value:**
  $$FV = P \times \left(\frac{(1 + r)^n - 1}{r}\right) \times (1 + r)$$
  *(where $P$ = monthly SIP, $r$ = monthly rate of return, $n$ = total months)*
- **Lumpsum / Future Value:**
  $$FV = P \times (1 + r)^t$$
- **Present Value:**
  $$PV = \frac{FV}{(1 + r)^t}$$

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- `pip` package manager

### Installation & Setup

1. **Clone the repository**
   ```bash
   git clone [https://github.com/shubhamharwani/](https://github.com/shubhamharwani/)<repo-name>.git
   cd <repo-name>
   ```

2. **Install dependencies**
   ```bash
   pip install streamlit pandas plotly babel
   ```
   *(Or if using a `requirements.txt` file: `pip install -r requirements.txt`)*

3. **Run the application**
   ```bash
   streamlit run app.py
   ```

---

## 🗺️ Roadmap & Planned Enhancements

- [ ] **Custom Inflation Rate:** Replace the fixed `6%` assumption with a user-adjustable inflation slider.
- [ ] **Step-Up SIP Mode:** Support annual percentage increases in monthly SIP contributions.
- [ ] **Year-by-Year Growth Chart:** Add a stacked area/bar chart showing invested capital vs. compounded returns over each year.
- [ ] **Goal-Based Reverse Calculator:** Allow users to enter a target corpus and solve for the required monthly SIP.

---

## ⚠️ Disclaimer

This application is built for educational and informational purposes only and does not constitute financial or investment advice.

---

## 👤 Author

**Shubham Harwani**  
- GitHub: [@shubhamharwani](https://github.com/shubhamharwani)  
- Instagram: [@oyesindhi_](https://instagram.com/oyesindhi_)
