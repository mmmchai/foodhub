# FoodHub Data Analysis
## Context
New York's restaurant scene is expanding rapidly, catering to busy students and professionals who rely on dining out or food delivery. FoodHub, a food aggregator, simplifies this with a single app connecting users to multiple restaurants.

Customers place orders through the app, which directs them to the restaurant. Once confirmed, a company-assigned delivery person picks up the order, navigates using the app, and delivers it to the customer. The app tracks each step, allowing customers to rate their experience. FoodHub earns revenue by taking a fixed commission from restaurant orders.

## Objective
To analyze order demand on the app and deliver data-driven recommendations to enhance the customer experience.

## Data Description
* order_id: Unique ID of the order
* customer_id: ID of the customer who ordered the food
* restaurant_name: Name of the restaurant
* cuisine_type: Cuisine ordered by the customer
* cost: Cost of the order
* day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
* rating: Rating given by the customer out of 5
* food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
* delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information

## Conclusions:
Revenue:

The top 5 restaurants contribute ~30% of total revenue, indicating a few major restaurants dominate the platform.
The 4 popular cuisines are American, Japanese, Italian, Chinese, which contribute over 80% of the total revenue. These cuisines drive most of the business on the platform.
Rating:

Among restaurants of the same cuisine type, highly-rated restaurants receives more order, indicating quality and customer satisfaction influence demand.
Cuisine types with high price do not guarantee high rating, indicating some restaurants may be overpriced, or did not provide high-than-par service quality to match its price points.
Customers are willing to pay slightly higher for highly-rated food.
Order Cost:

For the most popular cuisines (American, Japanese, Italian, Chinese), the average cost of these cuisines are close to the overall platform average. The median cost is skewed towards the lower end of the price range, which means more customers prefers budget friendly items on the menu, the higher priced items are ordered less frequently.
Mediterranean, Korean, and a few Vietnamese restaurants show significant price variation, suggesting inconsistent pricing strategies.
Furthermore, Korean and Vietnamese have the lowest price on average, however they are also one of the least popular cuisine types on this platform. This indicates that customers are also influenced by other factors besides price, such as service, portion size, food quality.
Delivery Time:

Delivery time significantly increases during the weekdays, while food preparation time remains constant between weekends or weekdays, suggesting potential bottleneck in delivery capacity during weekdays.
## Recommendations:
Revenue Strategy:

Leverage top-performing restaurants and form partnership strategies. Up-sell and cross-sell their menu items, since most customers are ordering budget-friendly items, but are willing to pay higher for high quality food. Promote top restaurants in the search results, provide discounts / promotions for higher-price items to drive adoption.

The promotions can be customized to each customer's purchase behaviour, or restaurants with higher ratings, as it is more likely for these restaurants to attract and retain new customers.

Incentivize customers to leave a rating.

Onboard new restaurants that specialize in popular cuisine types to capture additional customers.

For restaurants that have a high price but low rating, such as French and Southern, provide feedback to these restaurants.

Monitor pricing variability and reduce extreme pricing discrepancies.

Operation:

Further analyze the root cause for delivery bottleneck on weekdays, understand whether it varies by hour of the day due to peak demands during lunch and dinner time, or rush hour traffic.
