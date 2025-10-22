# 🧾 Consumer Behaviour and Shopping Pattern Analysis

![Image](https://github.com/user-attachments/assets/4772a729-acc0-4e61-bc7f-1dbda49334d7)

## 📘 Project Overview
This project explores **consumer shopping behaviour and purchasing patterns** using Microsoft Excel and PowerPivot.  
It seeks to uncover how various factors—such as **location, price, discounts, frequency, and payment methods**—influence customer purchasing habits and total sales revenue.

The dataset contains over **3,900 purchase records**, analyzed through **PowerPivot**, **PivotTables**, and **Regression Models**.

---

## 🎯 Business Questions Addressed

1. 🏷️ What is the **total revenue** of all purchased items across different locations?  
2. 🛒 What are the **total categories** of items purchased by consumers across locations?  
3. 💰 What are the **respective revenues** across these item categories?  
4. ⏰ What are the **most and least frequent purchase periods** (e.g., monthly, quarterly, annually)?  
5. 💳 What is the **distribution of payment methods** across product categories?  
6. 🚻 What is the **gender distribution** of customers?  
7. 📍 What are the **locations** from which purchases are made?  
8. 🚚 How frequent are the **shipping types** used in the delivery of products?  
9. 📉 Are **discounts applied** and **purchase amount** good predictors of **purchase frequency**?  
10. 🎟️ Is the **use of promo codes** a good predictor of purchase frequency?

---

## ⚙️ Tools & Techniques Used

| Tool | Purpose |
|------|----------|
| **Microsoft Excel** | Data cleaning, analysis, and visualization |
| **PowerPivot** | Data modeling, relationship management, DAX calculations |
| **Pivot Tables & Charts** | Summarization and pattern discovery |
| **Regression Analysis** | Testing predictor effects on purchase frequency |
| **Descriptive Statistics** | Summary of distributions and central tendencies |
| **Slicers & Conditional Formatting** | Dashboard interactivity and insights |

---

## 📊 Key Insights

- **Revenue Distribution:** Certain locations contributed significantly higher total revenue than others.  
- **Category Analysis:** Top-performing item categories varied by location and frequency.  
- **Purchase Frequency:** Monthly purchases were the most common; quarterly purchases were the least.  
- **Payment Behaviour:** Electronic transfers and debit card payments dominated across most categories.  
- **Gender Distribution:** Female customers made slightly more purchases than male customers.  
- **Predictive Insights:** Neither price nor discounts had a statistically significant effect on purchase frequency.

---

## 📈 Regression Analysis Summaries

### 🧮 Regression Model 1:  
**Dependent Variable:** Frequency of Purchase (DA)  
**Independent Variables:** Discounts Applied (DA) and Purchase Amount (PA in USD)

| Metric | Value |
|---------|-------|
| Multiple R | 0.01045 |
| R Square | 0.000109 |
| Adjusted R Square | -0.00040 |
| Standard Error | 34.6875 |
| Observations | 3,901 |

#### ANOVA
| Source | df | SS | MS | F | Significance F |
|---------|----|----|----|---|----------------|
| Regression | 2 | 512.29 | 256.15 | 0.2129 | 0.8083 |
| Residual | 3,898 | 4,690,166 | 1,203.22 | | |
| Total | 3,900 | 4,690,678 | | | |

#### Coefficients
| Variable | Coefficient | Std. Error | t Stat | P-value | Lower 95% | Upper 95% |
|-----------|--------------|-------------|----------|----------|-------------|-------------|
| Intercept | 28.1543 | 1.5909 | 17.6976 | **1.78E-67** | 25.0353 | 31.2732 |
| Discounts Applied (DA) | -0.5983 | 1.1219 | -0.5333 | 0.5939 | -2.7979 | 1.6013 |
| Purchase Amount (USD) | 0.0086 | 0.0235 | 0.3665 | 0.7140 | -0.0374 | 0.0546 |

🧩 **Interpretation:**
- The **R² = 0.0001** means the model explains less than 1% of variation in purchase frequency.  
- Both predictors (DA and PA) have **P-values > 0.05**, meaning they are **not statistically significant**.  
- Changes in price or discount **do not significantly affect** how often consumers buy.  

---

### 🧮 Regression Model 2:  
**Dependent Variable:** Frequency of Purchase  
**Independent Variable:** Price per Unit (PCU)

| Metric | Value |
|---------|-------|
| Multiple R | 0.00865 |
| R Square | 0.000075 |
| Adjusted R Square | -0.00018 |
| Standard Error | 34.6837 |
| Observations | 3,901 |

#### ANOVA
| Source | df | SS | MS | F | Significance F |
|---------|----|----|----|---|----------------|
| Regression | 1 | 350.71 | 350.71 | 0.2915 | 0.5893 |
| Residual | 3,899 | 4,690,327 | 1,202.96 | | |
| Total | 3,900 | 4,690,678 | | | |

#### Coefficients
| Variable | Coefficient | Std. Error | t Stat | P-value | Lower 95% | Upper 95% |
|-----------|--------------|-------------|----------|----------|-------------|-------------|
| Intercept | 28.6712 | 0.7356 | 38.9754 | **6.52E-281** | 27.2289 | 30.1134 |
| Price per Unit (PCU) | -0.6056 | 1.1216 | -0.5399 | 0.5893 | -2.8046 | 1.5934 |

🧩 **Interpretation:**
- **R² = 0.000075**, indicating negligible explanatory power.  
- The **p-value (0.589)** suggests **no significant relationship** between price per unit and frequency of purchase.  
- Therefore, changes in product price **do not meaningfully influence** how often customers buy.

- I'm always open to collaboration, feedback, or data-driven discussions!  
Feel free to connect with me or explore more of my work here on:
 GitHub  
 www.linkedin.com/in/christopher-owolabi-a920729a, 
 xto4success@gmail.com

---

## 📂 Repository Structure

