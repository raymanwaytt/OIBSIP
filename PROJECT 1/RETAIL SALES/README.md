## **Retail Sales Performance Analysis - Trends and Insights**

### **Executive Summary**
The retail business generated **$456K** in total revenue across **1,000 transactions**, maintaining an impressive average transaction value of **$456**. Operating across three distinct product categories—Electronics, Clothing, and Beauty—the business demonstrates a well-balanced revenue distribution with strong demographic engagement across various age groups and genders.

---

### **1. Data Exploration and Preparation**

#### **Initial Data Exploration (Python)**
- **Objective:** Understand the dataset and assess its quality.
- **Steps Taken:**
  1. Used `.isnull().sum()` to check for missing values in the dataset, ensuring data completeness.
  2. Leveraged `.describe()` to calculate descriptive statistics (e.g., mean, median, standard deviation) to gain insights into numerical columns.
- **Outcome:** Confirmed the dataset was clean and ready for analysis with no significant missing values.

#### **Data Transformation (Power BI)**
- **Objective:** Enhance the dataset with calculated columns to enable more in-depth analysis.
- **Steps Taken:**

  **1. Age Group:**
  - Created an Age Group column to categorize customers into ranges:
    ```DAX
    Age Group = 
    SWITCH(
        TRUE(),
        'retail_sales_dataset'[Age] >= 18 && 'retail_sales_dataset'[Age] <= 25, "18-25",
        'retail_sales_dataset'[Age] >= 26 && 'retail_sales_dataset'[Age] <= 35, "26-35",
        'retail_sales_dataset'[Age] >= 36 && 'retail_sales_dataset'[Age] <= 45, "36-45",
        'retail_sales_dataset'[Age] >= 46 && 'retail_sales_dataset'[Age] <= 55, "46-55",
        "56+"
    )
    ```

  **2. Age Group Sort:**
  - Added a sorting column to ensure Age Group categories were displayed in logical order:
    ```DAX
    Age Group Sort = 
    SWITCH(
        TRUE(),
        'retail_sales_dataset'[Age] >= 18 && 'retail_sales_dataset'[Age] <= 25, 1,
        'retail_sales_dataset'[Age] >= 26 && 'retail_sales_dataset'[Age] <= 35, 2,
        'retail_sales_dataset'[Age] >= 36 && 'retail_sales_dataset'[Age] <= 45, 3,
        'retail_sales_dataset'[Age] >= 46 && 'retail_sales_dataset'[Age] <= 55, 4,
        5
    )
    ```

  **3. Day of Week:**
  - Extracted the day of the week from the transaction date:
    ```DAX
    Day of Week = FORMAT(retail_sales_dataset[Date].[Date], "dddd")
    ```

- **Outcome:** The dataset was enhanced with Age Group, Age Group Sort, and Day of Week columns, enabling more targeted demographic and temporal analysis.

---

### **2. Revenue Analysis**

#### **Product Category Performance**

**Electronics Segment**
- **Total Revenue:** $157K (34.4% of total sales)
- **Average Revenue Per Sale:** $459
- **Units Sold:** 849
- **Price Per Unit:** $182
- **Market Position:** Category leader in revenue generation

**Clothing Segment**
- **Total Revenue:** $156K (34.1% of total sales)
- **Average Revenue Per Sale:** $443
- **Units Sold:** 894 (highest volume)
- **Price Per Unit:** $174
- **Market Position:** Volume leader with competitive pricing

**Beauty Segment**
- **Total Revenue:** $144K (31.5% of total sales)
- **Average Revenue Per Sale:** $467
- **Units Sold:** 771
- **Price Per Unit:** $184 (premium pricing leader)
- **Market Position:** Premium segment with highest per-unit pricing

---

### **3. Customer Demographics Analysis**

#### **Gender Distribution and Preferences**

**Female Customer Base**
- **Revenue Contribution:** $233.2K (51.06%)
- **Category Preferences:**
  - Strong preference for Beauty ($75K vs male $69K)
  - Leading in Clothing purchases ($81K vs male $74K)
  - Competitive in Electronics ($77K)

**Male Customer Base**
- **Revenue Contribution:** $223.2K (48.94%)
- **Category Preferences:**
  - Dominant in Electronics ($80K)
  - Significant participation in Clothing ($74K)
  - Growing presence in Beauty segment ($69K)

#### **Age Segment Analysis**

**Customer Distribution**

**46-55 Years (Prime Segment)**
- Largest customer group: 229 customers
- Average spending: $440
- Strong across all categories

**26-35 Years (Growth Segment)**
- Customer base: 205 customers
- Average spending: $480
- High engagement in Beauty and Electronics

**36-45 Years (Core Segment)**
- Customer base: 202 customers
- Average spending: $455
- Balanced category participation

**18-25 Years (Youth Segment)**
- Customer base: 169 customers
- Highest average spending: $500
- Strong affinity for Beauty and Electronics

**56+ Years (Mature Segment)**
- Average spending: $412
- Notable preference for Electronics

---

### **4. Temporal Analysis**

#### **Weekly Sales Patterns**

**Weekend Performance**
- **Saturday:** Peak revenue day ($525 average)
- **Sunday:** Moderate decline but sustained activity

**Weekday Performance**
- **Monday:** Strong start ($481 average)
- **Mid-week:** Stable performance
- **Friday:** Building momentum towards weekend peak

#### **Monthly Trends**
- Consistent transaction frequency throughout the year
- Notable seasonal variations in total monthly revenue
- Product category mix shows seasonal shifts
- Peak periods identified during summer months

---

### **5. Strategic Insights and Recommendations**

#### **Immediate Opportunities**

**Premium Pricing Strategy**
- Leverage Beauty segment's premium position
- Explore premium product lines in Electronics
- Develop luxury Clothing offerings

**Customer Engagement**
- Target high-spending youth segment
- Develop loyalty programs for 46-55 age group
- Create gender-specific marketing campaigns

**Operational Optimization**
- Strengthen Saturday staffing and inventory
- Optimize Monday opening operations
- Enhance mid-week promotional activities

#### **Long-term Strategic Initiatives**

**Product Development**
- Expand premium Beauty product lines
- Develop exclusive Electronics offerings
- Create targeted Clothing collections

**Market Expansion**
- Focus on high-potential age segments
- Develop cross-category promotional strategies
- Enhance gender-specific marketing

**Customer Experience**
- Implement personalized shopping experiences
- Develop omnichannel engagement strategies
- Create category-specific loyalty programs

---

### **6. Conclusion**
The business demonstrates robust performance with well-balanced revenue across categories and strong demographic engagement. The clear customer segmentation and temporal patterns provide multiple opportunities for targeted improvements and strategic adjustments. The high average transaction value and balanced category performance suggest a strong market position with significant potential for growth through strategic initiatives and targeted marketing efforts.

---

### **7. Key Performance Indicators (KPIs) for Future Monitoring**
- Category-specific revenue growth
- Age segment penetration rates
- Gender-based purchase patterns
- Weekend vs. weekday performance ratios
- Average transaction value trends
- Units sold per category
- Customer retention rates
- Seasonal performance variations
