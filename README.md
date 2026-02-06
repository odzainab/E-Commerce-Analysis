# E-Commerce Sales & Customer Loyalty Dashboard

_Uncovering how customer behavior, channels, and pricing strategies drive repeat purchases and long-term revenue growth._

---

## Quick Look

- **Total Sales:** $22.5M  
- **Growth:** +189.6% YoY  
- **Repeat Purchase Rate:** 100% (+6.2% YoY)  
- **Loyal Customer Revenue Share:** 35%–63% monthly  
- **Top Channel:** Website ($10.3M revenue)  
- **Refunds:** $635.7K (+171.9% YoY)  
- **Markdown Impact:** -$2.0M  
- **Top Discount Code:** WELCOME10 (32% repeat rate)  
- **Tools Used:** Power BI, Power Query
- **Dataset:** [View Dataset]()
- **Dashboard:** [View Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNWJhZjdlMjMtZmUzZS00N2UyLWJiOGUtMmZmZTU2N2QwNjc3IiwidCI6IjdlMGI1ZmNmLTEyYzQtNGVmZi05NmI2LTQ2NjRmMjVkYzdkYSIsImMiOjEwfQ%3D%3D)
- **Full Analysis:** [Medium](https://medium.com/@odzainab1/e-commerce-performance-analysis-strategies-for-boosting-revenue-and-loyalty-8515020ee1e1?postPublishedType=initial)


---

## Introduction

Revenue growth alone doesn’t sustain a business customer loyalty does. Businesses don’t lose money because sales are low; they lose money when customers stop coming back.

This project analyzes an e-commerce dataset from a global software retailer (Onyx Data November Challenge) to understand what drives repeat purchases, customer retention, and long-term revenue growth. Instead of focusing only on topline sales, the analysis centers on customer behavior the most reliable indicator of sustainable business success.

---

## Business Objective

- Identify loyal customers (repeat buyers)  
- Determine which channels, promotions, and pricing strategies drive repeat purchases  
- Build a single interactive dashboard that:
  - Tracks sales and loyal-customer trends over time  
  - Highlights revenue drivers and repeat-purchase behavior  
  - Shows how discounts and pricing impact performance  
  - Delivers actionable insights for business and stakeholder decision-making  

---

## Dataset & Tools

### Dataset 1: Events
- event_id, event_type, event_date  
- customer_id, product_id  
- region, country, channel, payment_method  
- quantity, unit_price, discount, net_revenue  
- refund indicators and reasons  

### Dataset 2: Customers
- customer_id, signup_date  
- region, country, acquisition_channel  
- segment, age_band  

### Dataset 3: Products
- product_id, product_name, category  
- subscription type, billing_cycle  
- base_price, vendor, release_date  

### Tools
- Power Query – Data cleaning and transformation  
- Power BI – Data modeling, DAX measures, and visualization  

---

## Data Preparation & Validation

1. **DimDate Table Creation**
   - Extracted Year, Month, Month Name, Day  
   - Created Month-Year fields  
   - Removed duplicates for accurate time analysis  

2. **Customer Purchase Count Dimension**
   - Grouped Events by customer_id  
   - Created PurchaseCount column  
   - Classified customers:
     - Loyal = ≥ 2 purchases  
     - Not Loyal = < 2 purchases  

3. **Data Cleaning**
   - Standardized data types  
   - Replaced missing regions and refund reasons with “N/A”  
   - Removed duplicate and invalid rows  

4. **Relationships**
   - Customer → Events  
   - Product → Events  
   - Events → DimDate  
   - Customer → Purchase Count  

This structure supports scalable behavioral analysis, loyalty segmentation, and time-based performance tracking.

---
## Data Visualization

![E-commerce real_page-0001](https://github.com/user-attachments/assets/ff9c47e6-ccd4-4677-b226-7e5701db3755)

![E-commerce real_page-0002](https://github.com/user-attachments/assets/bc5e57f0-c481-4817-bd72-0e0b5b3dc513)


![E-commerce real_page-0003](https://github.com/user-attachments/assets/cbaf580e-f427-4c45-83b8-7241016b4d02)


## Key Insights

- **Explosive Growth, Retention-Led:** Sales reached $22.5M (+189.6% YoY) driven primarily by repeat customers, not customer acquisition.
- **Perfect Repeat Purchase Rate:** 100% of customers made at least one repeat purchase, signaling strong product-market fit and retention.
- **Loyal Customers Drive Revenue:** Loyal customers contribute 35%–63% of monthly revenue, peaking mid-year.
- **Website Dominance:** The website is both the top revenue channel and the largest source of loyal customers.
- **Regional Pricing Differences:** ASP varies significantly by country, indicating strong potential for localized pricing strategies.
- **Rising Refund Risk:** Refunds increased 171.9% YoY, largely driven by billing errors and accidental purchases.
- **Margin Pressure from Markdowns:** Aggressive discounting (-$2.0M) is eroding margins.
- **Subscription-Led Revenue:** 98% of products sold are subscriptions, with annual plans massively outperforming monthly.
- **High-Impact Add-Ons:** Add-ons such as Team Seats and Zoom Whiteboard drive strong cross-sell and AOV growth.
- **Discounts That Drive Loyalty:** The WELCOME10 code delivers the highest repeat purchase rate (32%).

---

## Recommendations

1. **Shift Growth Strategy Toward Acquisition** – Scale new customer acquisition while maintaining strong retention.
2. **Convert Monthly to Annual Subscribers** – Use incentives and feature gating to drive higher ARPC and revenue stability.
3. **Fix Refund Drivers** – Audit checkout and billing processes to reduce refund volume and customer friction.
4. **Replace Blanket Discounts with Targeted Promotions** – Use bundles, loyalty rewards, and time-limited offers instead of constant markdowns.
5. **Double Down on High-Performing Products & Add-Ons** – Bundle underperforming products with top sellers to diversify revenue.
6. **Shorten Time to Second Purchase** – Trigger follow-ups and offers within the first 2–3 weeks after purchase.
7. **Re-Engage Loyal Customers During Off-Peak Months** – Launch loyalty-exclusive campaigns to stabilize seasonal dips.

---

## Next Steps

- Build acquisition pipelines targeting high-potential regions  
- Launch experiments to convert monthly users to annual plans  
- Redesign checkout and billing workflows  
- Implement smarter inventory and pricing controls  
- Track loyalty and refund trends continuously  

---

## Conclusion

The business is experiencing exceptional revenue growth driven by strong customer loyalty and repeat purchases. However, stagnating acquisition, rising refunds, and margin erosion from aggressive markdowns present strategic risks.

By shifting toward value-driven growth through smarter pricing, improved acquisition, reduced refund friction, and stronger loyalty engagement  the business can sustain long-term profitability and market leadership.

