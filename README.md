# AB-Test-Conversion-Analysis-on-Web-Design
# 1. Introduction
For this project, we will be analyzing the results of an A/B test run by an e-commerce website. The final goal is to help the company understand if they should implement the new page, keep the old page, or perhaps run the experiment longer to make their decision

# 2. Import data & data cleaning

# 3. Analyze results
Let's assume that the new page does not have higher conversion rate than the old page at 5% Type I error. So the hypothesis woule be:

null: 𝑝𝑛𝑒𝑤 - 𝑝𝑜𝑙𝑑 <=0
alternative: 𝑝𝑛𝑒𝑤 - 𝑝𝑜𝑙𝑑 >0

# 3.1 Z-test in our way
<img width="309" alt="image" src="https://github.com/kyang18/AB-Test-Conversion-Analysis-on-Web-Design/assets/76982420/7101195a-137f-477e-9bb2-eb275941a9cb">
<img width="907" alt="image" src="https://github.com/kyang18/AB-Test-Conversion-Analysis-on-Web-Design/assets/76982420/b1765797-f1b9-403c-9d4a-ed2b59d28701">

p-value is less than 0.05, so we can reject null hypothesis and accept alternative hypothesis that 𝑝𝑛𝑒𝑤 - 𝑝𝑜𝑙𝑑 >0, the new page has higher conversion rate than the old page

# 3.2 Z-test in Statsmodels
<img width="896" alt="image" src="https://github.com/kyang18/AB-Test-Conversion-Analysis-on-Web-Design/assets/76982420/9511b929-b30f-4d01-ab2f-a3325b2e4b37">

p-value is less than 0.05, so we can reject null hypothesis and accept alternative hypothesis that 𝑝𝑛𝑒𝑤 - 𝑝𝑜𝑙𝑑 >0, the new page has higher conversion rate than the old page
