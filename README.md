# Проект 1. Ріст Реальної Ціни На Житло
В даному проекті розглянуто відсоткова зміна реальної ціни на житло протягом 2013 – 2023 року. Наша ціль, знайти країну з найбільшим ростом в ціні, щоб довгострокові інвестиції в житлову нерухомість принесла максимум  прибутку.
Для цього було знайдено середні відсотки по рокам по кожній країні, щоб знайти топ 5 країн з найбільшим показником. 

Дашборди та візуалізація (Power BI) [here](https://app.powerbi.com/view?r=eyJrIjoiOWQ1YzllMWItMWY3NC00MzA1LWFlMzgtMTEyOGUwNDk1NDgzIiwidCI6ImQ0NTFiZGY3LTVkNjgtNGFiOS05MTY1LTc5NGVkZGJhZTBmYSIsImMiOjl9)
<details>
   <summary> Більше </summary>

## Загальна інформація про структури даних (Data structure overview)

Така таблиця була використана: real-year<br/>
Туди входили такі колонки: <br/>
Date(date) – дата встановленої ціни на житло поквартально<br/>
Country(string) – 59 країн світу <br/>
Price(numeric) – ціна на житло <br/>

|**Table**     |   **real_year**  |
|--------------|------------------|
| Country      | VARCHAR(255)     |
| Date         | DATE             |
| Price        | DECIMAL(10,2)    |

Дані були взяті з [сайту](https://datahub.io/core/house-prices-global#readme)

## Короткий огляд (Executive summary)
В результаті дослідження, було визначено крани з найбільшим середнім показником росту ціни на житло протягом 10 років. <br/> Туди ввійшли: <br/>
Туреччина – 10,38% <br/>
Угорщина – 5,89% <br/>
Ісландія – 5,89% <br/>
Ірландія – 5,66% <br/>
Португалія – 5,16%<br/>
В останні роки Туреччина мала високий підйом в ціні, це було спричинено високою інфляцією та спробою зберегти свої заощадження в купівлі житлової нерухомості. 
Інші країни в топ 5 мають нормальну волатильність, тому в їх можна інвестувати.

## Глибокий аналіз інсайтів (Insights deep dive)
В [таблиці та графіку](https://app.powerbi.com/view?r=eyJrIjoiOWQ1YzllMWItMWY3NC00MzA1LWFlMzgtMTEyOGUwNDk1NDgzIiwidCI6ImQ0NTFiZGY3LTVkNjgtNGFiOS05MTY1LTc5NGVkZGJhZTBmYSIsImMiOjl9)
 відображені країни з найбільшим високим середнім відсотком, протягом 10 років (2013-2023 р.). З даної інформації видно, що найбільший ріст реальної ціни на житло протягом зазначеного часу був у Туреччині, Угорщині, Ісландії, Ірландії та Португалії.

<img width="974" height="557" alt="image" src="https://github.com/user-attachments/assets/45545c54-cc3d-47d2-a5eb-864727cce5b9" />
Факти, які повпливали на ріст: <br/>
- Ціни на житло виросли в рази за останні роки в Туреччині через високу інфляцію, яка склала 48.7% за 2022 рік, в 2023 році вона сягнула 64.7%. Також багато людей бажають вкластися в нерухомість, щоб зберегти свої кошти, тому на графіку можна помітити значний ріст в дані роки.<br/> 
- Угорщина – має вплив на підвищення цін, через нестачу житла, низькі іпотечні та податкові ставки. Також ця країна є популярною серед туристів.<br/>
- Ісландія має проблему з житловою кризою, тобто з нестачею житла для всього населення.<br/>
- Ірландія - має дефіцит пропозиції житла та одну з найбільш економічно зростаючих економік Європи.<br/>
- Португалія – мають програму «золота віза», яка вплинула на попит з боку іноземних інвесторів. Також на ріст цін вплинули: обмеження пропозицій на ринку та збільшення туризму.<br/>


## Рекомендації (Recommendations)
В даній ситуації краще не інвестувати в Туреччину, адже на графіку видно, що загальний відсоток росту ціни великий тільки через те, що в 2022-2023 році інфляція в Туреччині було високою. <br/>
Менш ризиковіше буде інвестувати в Угорщину, Ісландію, Ірландію та Португалію. Вони мають не значну волатильність та достатньо високий сердній зростаючий відсоток. 

</details>

# 2nd Project. State Expenditures During the War
Ukraine is at war, and in recent years the situation has worsened, which is why budget expenditures were expected to increase, especially defense spending.<br/>
Our goal is to determine whether defense spending has increased, its ranking among other spending categories, and its share of total expenditures.
We will also examine whether the state has sufficient resources to cover expenses based on the received state revenue.<br/>
Dashboard [here](https://app.powerbi.com/view?r=eyJrIjoiMzIzZDE5NTYtMTgyYi00YzQzLThhZGItNTA0NjkxZTIwMzYwIiwidCI6ImQ0NTFiZGY3LTVkNjgtNGFiOS05MTY1LTc5NGVkZGJhZTBmYSIsImMiOjl9)

<details>
   <summary> More </summary>
   
## Data structure overview
Two tables were used for analysis: budget and state_revenue.<br/>
Structure of the first table – budget:<br/>
•	date — monthly expenses for each sector from 2022 onward<br/>
•	public_ord — public order and judicial authorities<br/>
•	econom_activity — economic activity<br/>
•	national_funct — general government functions<br/>
•	defense — defense spending<br/>
•	dept_service — debt servicing<br/>
•	education — education spending<br/>
•	healthcare — healthcare spending<br/>
•	social_pro — social protection<br/>
Structure of the second table – state_revenue:<br/>
•	year — year<br/>
•	revenue — state budget income<br/>

<img width="703" height="481" alt="image" src="https://github.com/user-attachments/assets/f68da903-4312-4d13-a1b8-2b755d0fa85a" />

Expenditure data source [here](https://opendatabot.ua/war)<br/>
Revenue data source [here](https://index.minfin.com.ua/ua/finance/budget/gov/income/2022/)<br/>


## Executive summary
Between 2022 and 2024, defense expenditures ranged from 39% to 48% of total expenditures, making it the largest category.
In 2023, defense spending increased significantly by 84.5%, while in 2024, the growth was only 9.9%.<br/>
The state struggles to cover its expenses—almost all annual revenue goes to defense.

## Insights deep dive
### Expenditures by Year
Over the past three years, defense spending has remained the highest among all expenditure categories. Public order and social protection ranked second and third, respectively. In 2022, defense expenditures amounted to UAH 1,137 billion; in 2023 — UAH 2,098 billion; and in 2024 — UAH 2,305 billion.<br/>
As of 2025, data is already available for the first five months, showing UAH 1,125.4 billion spent on defense. If we divide this amount by five and project it for twelve months, the estimated annual expenditure would be around UAH 2,700 billion. This suggests that spending in this sector is likely to continue increasing.

<img width="974" height="527" alt="image" src="https://github.com/user-attachments/assets/cf67f1a5-8a0c-4df6-8685-a5f3c9df6c4a" />

### Structure of Defense Spending (2022–2024)
Defense consistently made up more than one-third of all expenditures:<br/>
2022: 39.4%<br/>
2023: 48.5%<br/>
2024: 47.8%<br/>
Comparing 2022 and 2023:
+84.5% growth<br/>
From 2023 to 2024:<br/>
Only +9.9% growth<br/>
Considering inflation >10% in 2024, real growth was negligible.
The significant increase occurred between 2022 and 2023 only.
Even adjusted: 84.5% - 25% inflation ≈ 59.5% effective growth.

### Government Revenue and Expenditures
The state has much higher expenditures than income, with defense spending nearly equaling total revenue.
Thus, the budget is running a deficit, which negatively affects the economic condition and may increase monetary emission to cover growing defense needs.
</details>

# 3rd Project. A/B Test
An A/B test was conducted by a company that launched two campaigns:<br/>
•	Control Campaign<br/>
•	Test Campaign<br/>
Their goal was to increase the number of actual customers.
My goal was to determine whether the test campaign showed success over the course of a month.
So, I compared key metrics to understand whether:<br/>
•	more customers came from the reach in the test campaign,<br/>
•	the percentage of reach among total impressions was higher,<br/>
•	the spending on the test campaign was effective.<br/>

<details>
   <summary> More </summary>
   
## Data structure overview
A/B testing helps in finding a better approach to finding customers, marketing products, getting a higher reach, or anything that helps a business convert most of its target customers into actual customers. <br/>
Below are all the features in the dataset:<br/>
•	Campaign Name: The name of the campaign<br/>
•	Date: Date of the record<br/>
•	Spend: Amount spent on the campaign in dollars<br/>
•	of Impressions: Number of impressions the ad crossed through the campaign<br/>
•	Reach: The number of unique impressions received in the ad<br/>
•	of Website Clicks: Number of website clicks received through the ads<br/>
•	of Searches: Number of users who performed searches on the website<br/>
•	of View Content: Number of users who viewed content and products on the website<br/>
•	of Add to Cart: Number of users who added products to the cart<br/>
•	of Purchase: Number of purchases<br/>
Two campaigns were performed by the company:<br/>
•	Control Campaign<br/>
•	Test Campaign<br/>

 <img width="612" height="628" alt="image" src="https://github.com/user-attachments/assets/8a30aaaa-9970-479c-8399-974ebd8d91f2" />

Data set [here](https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset/data)

## Executive summary
The company ran an A/B test with two different ad campaigns lasting one month. The first was a regular campaign (control), and the second was a new version (test campaign).<br/>
The control campaign proved to be more successful. It required less budget ($67K), reached a wider audience, and delivered better results in terms of customers per dollar spent, attracting approximately 17 customers.<br/>

## Insights deep dive
The company ran one ad campaign as usual (Control Campaign), and the other with a new strategy (Test Campaign).
The Control Campaign spent $67K, and the Test Campaign spent $77K.
Even though the Test Campaign had higher costs and lower reach, the ad attracted more interest.
Despite the higher spending, the test campaign reached fewer people overall. While the test ad generated more interest per viewer, it did not translate into better performance — more purchases came from the control campaign.

<img width="974" height="541" alt="image" src="https://github.com/user-attachments/assets/c6c2e441-02cb-4baf-a325-d316c2396e5c" />

### % of Customers from Reach
The percentage of customers from the total reach during the ad campaign was higher in the Test Campaign.
On some days, the metric exceeded 5%, which is a very good result — especially when compared to the Control Campaign where it stayed below 4%, though more stable.

### % of Unique Views from Total Impressions
The table provided information on total impressions and unique reach.
It’s important for more potential clients to see the product within the allocated budget.
The Control Campaign had 81% unique views, while the Test Campaign had 71.7%.
So, the higher percentage in the Control Campaign shows it was more efficient.

### Purchases per $1
Ultimately, more customers were acquired during the control campaign, as it showed a higher number of customers per dollar spent, outperforming the test campaign by about 7 customers.

**In conclusion**, the Test Campaign was successful:
The control campaign outperformed the test campaign in key performance areas:<br/>
•	It spent less money <br/>
•	Reached more people <br/>
•	Showed stable customer inflow indicators <br/>
As a result, it stands out as the more effective advertising strategy.<br/>


</details>


