# The Anchoring Paradox: Pricing and Trust in Pakistan’s E-Commerce Market

Dataset Used: https://www.kaggle.com/datasets/zusmani/pakistans-largest-ecommerce-dataset?resource=download

### Project Overview

Standard economic theory suggests that the **Anchoring Effect** is a universal driver of sales. This is the idea that consumers "anchor" to a high original price, making a lower sale price feel like a bargain. However, in markets with low institutional trust, this logic can fail.

I analyzed over **584,000 transaction records** from a major Pakistani e-commerce platform to test if discounts actually increase purchase volume. The data reveals a significant "Trust Deficit." In many categories, aggressive discounting actually causes consumers to buy less, as they interpret the lower price as a signal of low quality.

### Key Analytical Findings

#### 1. The Aggregate Trust Gap

Across the entire dataset, flat-priced items outperformed discounted ones. On average, shoppers bought **1.22 units** per order at full price, compared to only **1.10 units** when a sale was applied.

<img width="567" height="476" alt="image" src="https://github.com/user-attachments/assets/3fbd9250-5d7a-429c-b3b0-5382d41a665f" />


*This graph shows that stable pricing generally commands higher order volumes than promotional pricing.*

#### 2. The Premium Paradox

The "Trust Deficit" is most extreme when the financial stakes are high. Using a three-tier price segmentation (Low, Mid-Range, and High), the data shows that premium buyers actively avoid sales.

* **High-Segment Shoppers:** Order volume dropped from **1.43 units** at full price to **1.08 units** when discounted.
* **Economic Interpretation:** For expensive goods, price acts as a signal of authenticity. A steep discount triggers "The Market for Lemons" theory, where buyers assume the product is fake or defective.

<img width="846" height="530" alt="image" src="https://github.com/user-attachments/assets/601d1eed-02cf-4b1b-8365-5686a2b41243" />


*Luxury and high-end shoppers show the sharpest rejection of discount tags.*

#### 3. The "Lipstick Effect" Anomaly

There is a notable exception in the **Beauty & Grooming** category. This is the only major segment where the standard Anchoring Effect works as intended: sale items (**1.46 units**) outsold flat-priced items (**1.30 units**). Because these are low-risk, high-gratification purchases, the fear of a "lemon" is lower, allowing the bargain incentive to take over.

<img width="1001" height="640" alt="image" src="https://github.com/user-attachments/assets/82653c31-78cb-46b9-8c05-24c8028ab9fa" />


*Beauty products stand out as the primary category where discounts successfully drive volume.*

#### 4. Payment Method as a Proxy for Trust

The root cause of this behavior lies in how people pay.

* **Bank/Card Users:** These digital shoppers trust the platform. Their behavior is indifferent to sales (P-Value: 0.45), meaning they buy what they need regardless of marketing tricks.
* **Cash on Delivery (COD) Users:** These shoppers are inherently skeptical. The statistical proof is definitive (T-Statistic: -9.68). COD buyers significantly reduce their order sizes when they see a discount, viewing it as a red flag for a potential scam.


<img width="846" height="547" alt="image" src="https://github.com/user-attachments/assets/95489c71-d87d-4473-9043-348559c1e74e" />


*COD users, representing the majority of the cash economy, are the primary drivers of the trust deficit.*

### Statistical Robustness

To ensure these findings were not random noise, I conducted **T-Tests** on the populations. The overall market results and the COD results showed P-Values of **0.0000**, proving that the "Trust Deficit" is a statistically significant market pattern in Pakistan.

### Strategic Recommendations

Based on this analysis, businesses operating in Pakistan should consider the following:

* **Maintain Price Integrity:** For high-value goods like electronics or premium fashion, a stable, "fair" price builds more brand equity than constant flash sales.
* **Segment Your Sales:** Reserve aggressive discounting for low-risk categories (Cosmetics, Consumables) where consumer trust is already established.
* **Incentivize Digital Payments:** Shifting users toward digital banking is a behavioral "unlock" that allows standard promotional tools to finally become effective.


### Technical Stack

* **Language:** Python
* **Libraries:** Pandas, Matplotlib, SciPy

### How to Run

1. Clone this repository.
2. Ensure you have the `Pakistan Largest Ecommerce Dataset.csv` in the root folder.
3. Open `Anchoring_Trap.ipynb` in a Jupyter environment or VS Code.
4. Run all cells to reproduce the statistical analysis and visualizations.
