# 📧 Email Subject Line A/B Testing for E-commerce Campaigns

![Email Marketing](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns/Image/email-marketing.jpg)

📂 **Full Analysis Available in Jupyter Notebook:** [here📒](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns.ipynb)

📂 **Check Presentation in PDF:** [here📒](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns.pdf)

📂 **Check Presentation in PowerPoint:** [here📒](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns.pptx)

This project analyzes the impact of different email subject line strategies—**Personalized** and **Urgency-based**—on key email marketing metrics: **Open Rate**, **Click-Through Rate (CTR)**, and **Conversion Rate**. The goal is to determine which subject line strategy performs best in engaging users and driving conversions.

---

## 🎯 Purpose of the Project

The success of an email marketing campaign largely depends on the effectiveness of the subject line. This project aims to:
- Identify the most effective subject line strategy that increases user engagement.
- Optimize email marketing performance by making data-driven decisions.
- Boost conversion rates through impactful subject lines.

---

## 🚨 Problem Statement

Many e-commerce businesses struggle with low engagement in email marketing. Users often ignore or delete promotional emails without opening them. This project investigates whether a **Personalized** subject line or an **Urgency-based** subject line performs better.

---

## 💡 Rationale of the Project

Choosing the right subject line can significantly impact a company's revenue. This study provides actionable insights for marketers to:
- Improve email open rates to maximize reach.
- Increase CTR (Click-Through Rate) to drive traffic to landing pages.
- Enhance conversion rates to boost sales.

---

## 📊 Subject Line Variants and Examples

### 1. **Personalized Subject Lines**
Tailored to the recipient's name, past behavior, or preferences.  
- Example: *"John, your exclusive offer is waiting! 🎉"*  
- Expected Outcome: Increased engagement by making the email feel relevant.

### 2. **Urgency-Based Subject Lines**
Creates a sense of urgency or scarcity.  
- Example: *"Hurry! Your 50% discount expires in 3 hours! ⏳"*  
- Expected Outcome: Drives immediate action due to FOMO (Fear of Missing Out).

---

## 📐 Hypothesis Statements

| Metric               | Null Hypothesis (H₀)                                                                 | Alternative Hypothesis (H₁)                                                                 |
|----------------------|---------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|
| **Open Rate**        | There is no significant difference in open rates between variants.                    | Personalized subject lines result in higher open rates.                                      |
| **CTR (Click-Through Rate)** | There is no significant difference in CTR between variants.                          | Urgency-based subject lines result in higher CTR.                                            |
| **Conversion Rate**  | There is no significant difference in conversion rates between variants.              | Urgency-based subject lines result in higher conversion rates.                               |

---

## 📊 Data Collection and Metrics

I conducted an A/B test using real email campaign data from an e-commerce business.

📊 **Dataset:** `email_campaign_data.csv`  
📌 **Total Records:** 500,000 emails  
📌 **Fields in Dataset:**  

| Column Name       | Description  |
|------------------|--------------|
| `customer_id`       | Unique ID for each email sent |
| `first_name` | Name of the customer |
| `email_sent_date` |date when the email was sent |
| `subject_line_variant` | Subject line type (*Personalized* or *Urgency*) |
| `email_opened`         | 1 if email was opened, 0 if not |
| `link_clicked`        | 1 if a link was clicked, 0 if not |
| `purchased_made`      | 1 if a purchase was made, 0 if not |

🔗 **Check the Dataset:** [email_campaign_data.csv](https://github.com/jimi121/PYTHON-PROJECTS/blob/main/Email%20Subject%20Line%20AB%20Testing%20for%20E-commerce%20Campaigns/email_marketing.csv)   


### Key Metrics:
- **Open Rate**: $(\text{Emails Opened} / \text{Emails Sent}) \times 100\%$  
- **CTR (Click-Through Rate)**: $(\text{Clicks} / \text{Opened Emails}) \times 100\%$  
- **Conversion Rate**: $(\text{Purchases} / \text{Clicks}) \times 100\%$

### Sample Sizes:
- Total emails sent: $ N = 100,000 $
- Split evenly between groups: $ N_{\text{Personalized}} = 50,000 $, $ N_{\text{Urgency}} = 50,000 $

---
## 📈 Results and Visualization

### 1. Email Performance Comparison by Subject Line Variant

#### Bar Chart Comparison:
Below is a bar chart comparing the performance of the two subject line strategies across the three key metrics:

![Bar Chart Comparison](https://via.placeholder.com/600x400?text=Bar+Chart+Comparison)

| Metric               | Personalized (%) | Urgency (%) | Winner          |
|----------------------|------------------|-------------|-----------------|
| **Open Rate**        | 44.8             | 40.2        | 🟩 Personalized |
| **CTR**              | 18.0             | 22.2        | 🟩 Urgency      |
| **Conversion Rate**  | 0.6              | 1.1         | 🟩 Urgency      |

---

### 2. Statistical Significance Tests

#### A/B Test for Open Rate:
To validate the Open Rate difference statistically, we performed a hypothesis test using the Z-test formula:

$$
Z = \frac{\bar{X}_1 - \bar{X}_2}{\sqrt{\frac{\sigma_1^2}{n_1} + \frac{\sigma_2^2}{n_2}}}
$$

Where:
- $\bar{X}_1$: Mean Open Rate for Personalized ($44.8\%$)
- $\bar{X}_2$: Mean Open Rate for Urgency ($40.2\%$)
- $\sigma_1^2$, $\sigma_2^2$: Variances of the two groups
- $n_1$, $n_2$: Sample sizes ($50,000$ each)

**Results:**
- $Z = 33.38$
- Critical value at $\alpha = 0.05$: $±1.96$

**Interpretation:**
The Z-score is far beyond the critical threshold ($±1.96$). The difference in open rates is statistically significant. Personalized subject lines are significantly better for driving email opens.

#### Normal Distribution Visualization:
![Open Rate Normal Distribution](https://via.placeholder.com/600x300?text=Open+Rate+Normal+Distribution)

---

#### A/B Test for CTR (Click-Through Rate):
We ran another hypothesis test for CTR using the same Z-test formula.

**Results:**
- $Z = -24.25$
- Critical value at $\alpha = 0.05$: $±1.96$

**Interpretation:**
The Z-score is far beyond the rejection region. Urgency-based subject lines drive significantly higher CTR.

#### Normal Distribution Visualization:
![CTR Normal Distribution](https://via.placeholder.com/600x300?text=CTR+Normal+Distribution)

---

#### A/B Test for Conversion Rate:
Finally, we tested for Conversion Rate.

**Results:**
- $Z = -17.60$
- Critical value at $\alpha = 0.05$: $±1.96$

**Interpretation:**
The Z-score falls within the rejection region. Urgency-based subject lines lead to more conversions.

#### Normal Distribution Visualization:
![Conversion Rate Normal Distribution](https://via.placeholder.com/600x300?text=Conversion+Rate+Normal+Distribution)

---

## 📌 Insights and Recommendations

### Key Takeaways:
- **Personalized subject lines** excel in **Open Rates**, meaning users find them more engaging.
- **Urgency-based subject lines** drive higher **CTR** and **conversions**, leading to more sales.
- Statistical testing confirms that these differences are significant and not due to randomness.

### Actionable Recommendations:
- ✅ Use **Personalized Subject Lines** to maximize email opens.  
  - Example: *"Sarah, your exclusive deal is inside!"*  
- ✅ Incorporate **Urgency** in follow-up emails to drive clicks and purchases.  
  - Example: *"Only 2 hours left to claim your 50% discount!"*  
- ✅ Combine both strategies for maximum impact!  
  - Example: *"Mark, your VIP deal expires in 1 hour! ⏳"*  
- ✅ Test different subject lines regularly to continuously optimize campaigns.

---

## 🎉 Conclusion

This A/B testing project provided clear insights into how subject lines influence email engagement and conversions. Personalization helps increase open rates, while urgency-based messaging drives action. By implementing these findings, e-commerce businesses can significantly improve their email marketing performance and increase sales.

---

## 🤝 Final Thoughts

This project showcases the power of data-driven marketing. With the right subject line, businesses can increase customer engagement, improve conversions, and drive revenue growth. 📈🚀
