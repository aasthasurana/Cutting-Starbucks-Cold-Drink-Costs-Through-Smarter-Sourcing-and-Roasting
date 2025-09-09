# ☕ Cutting Starbucks’ Cold Drink Costs Through Smarter Sourcing and Roasting

This project develops a **linear programming optimization model** to minimize Starbucks’ coffee sourcing, roasting, and transportation costs while meeting demand and quality thresholds. With cold beverages now accounting for **75% of U.S. sales**, the model explores the strategic use of **Robusta beans** (cheaper, more resilient) alongside Arabica to reduce costs without compromising brand equity.

---

## 📌 Problem Statement & Motivation
- Arabica prices surged to **$4.40/lb in 2024** (47-year high) due to climate disruptions.  
- Starbucks cold drinks, less sensitive to bean quality, present an opportunity for **strategic Robusta blending**.  
- Objective: Minimize total system cost of producing **100M+ beverages annually** while maintaining quality, roast balance, and operational feasibility.  

---

## 🛠️ Optimization Model
**Decision Variables:**  
- **Bean Mix:** Arabica vs. Robusta for hot and cold drinks  
- **Roast Mix:** Blonde, Medium, Dark  
- **Origin Sourcing:** Brazil, Colombia, Ethiopia, Vietnam  
- **Transport Modes:** Air, Ocean, Land  
- **Inventory:** Storage buffer  

**Constraints:**  
- Hot drinks ≥ 85% Arabica (max 15% Robusta)  
- Cold drinks: Robusta allowed up to 100%  
- Roast balance: Blonde ≤ 30%; medium & dark required  
- Each origin ≤ 40% of Arabica supply  
- Transport: At least 10% via air, land, and ocean  
- Minimum 20% inventory buffer  

**Objective Function:**  
Minimize:  
- Bean sourcing costs  
- Roasting costs  
- Transportation costs  
- Inventory holding costs  

---

## 📊 Key Results
- **Optimal Cost:** $16.6M vs. $21M all-Arabica baseline → **$5M annual savings**  
- **Optimal Blend:**  
  - Hot drinks: 85% Arabica, 15% Robusta  
  - Cold drinks: 100% Robusta  
- **Roast Mix:** 60% Medium, 30% Blonde, 10% Dark  
- **Transport:** 80% Ocean, 10% Land, 10% Air  
- **Origins:** Diversified across Brazil, Colombia, and Ethiopia  

---

## 💡 Business Implications
- **Cost Reduction:** Saves $5M–5.5M annually by optimizing bean mix and logistics  
- **Supply Chain Resilience:** Diversifies origins and ensures 20% inventory buffer  
- **Consumer-Centric Blending:** Maintains Arabica dominance in hot drinks to preserve brand equity  
- **Efficient Logistics:** 80% ocean shipping reduces cost; air/land transport ensures freshness  

---

## 📈 Sensitivity & Scenario Analysis
- Relaxing Arabica requirement in hot drinks (85% → 60%) saves **up to $495K**  
- Higher Arabica prices significantly increase total cost (+$748K at $6.0/lb)  
- Arabica in cold drinks is always avoided due to cost inefficiency  
- Inventory and transport constraints add resilience but increase cost  

---

## 🛠️ Tools & Libraries
- Python: `pandas`, `numpy`, `pyomo` / `PuLP`, `matplotlib`  
- Excel Solver (early testing)  
- Linear Programming & Sensitivity Analysis  

---
