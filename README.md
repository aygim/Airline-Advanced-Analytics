# Airline Advanced Analytics & Customer Revenue Analysis

## Project Overview

This project analyzes airline booking, ticket, flight, customer, route, and aircraft data to explore customer behavior, revenue performance, and operational patterns.

The analysis combines **SQL, Python, statistical testing, and machine learning** to transform relational airline data into business insights.

The project focuses on questions such as:

- Which customers generate the most revenue?
- Which routes contribute the most to revenue?
- How does ticket pricing differ across fare classes?
- Are there statistically significant differences in ticket revenue across customer and aircraft groups?
- Can customers be segmented based on their value and transaction behavior?

---

## Tools & Technologies

- **SQL / SQLite** — data extraction, joins, aggregations, CTEs, and business metric calculations
- **Python** — data analysis and statistical testing
- **Pandas & NumPy** — data cleaning, transformation, and exploratory analysis
- **SciPy** — statistical hypothesis testing
- **scikit-learn** — customer segmentation and feature scaling
- **Plotly** — interactive data visualization
- **Jupyter Notebook** — analysis and documentation

---

## Dataset

The project uses a relational airline database containing information about:

- Customers and passengers
- Bookings
- Tickets
- Flights
- Ticket-flight transactions
- Airports and routes
- Aircraft and seating
- Boarding passes

The database contains more than **1 million ticket-flight records**, providing enough transactional data for customer, route, fare-class, and revenue analysis.

---

## Analysis Workflow

### 1. Data Exploration & Validation

The first stage focused on understanding the structure and quality of the data.

Key steps included:

- Reviewing database tables and relationships
- Checking record counts
- Identifying missing values
- Reviewing unique identifiers
- Validating booking and flight date ranges
- Examining relationships between customers, bookings, tickets, and flights

These checks helped establish a reliable foundation for the subsequent analysis.

---

### 2. Customer Revenue Analysis

SQL queries were used to combine customer, booking, ticket, flight, and airport information.

Customer-level metrics included:

- Total customer spending
- Number of flights
- Number of tickets
- Average ticket value
- Maximum ticket value
- Revenue per flight
- Number of cities visited

This analysis helped identify high-value customers and understand differences in customer spending behavior.

---

### 3. Route Revenue Analysis

Route-level analysis was performed to understand revenue performance across the airline network.

Metrics included:

- Number of flights
- Tickets sold
- Total route revenue
- Average ticket price
- Revenue per flight
- Seat occupancy estimates

The analysis helped identify routes with strong revenue contribution and differences in route performance.

---

### 4. Fare Class Analysis

Ticket performance was analyzed across fare classes, including:

- Economy
- Business
- Comfort

The analysis compared:

- Tickets sold
- Total revenue
- Average ticket price
- Revenue contribution by fare class

This provided insight into how passenger volume and ticket value contribute differently to overall airline revenue.

---

## Statistical Analysis

### Business vs. Economy Ticket Prices

A **two-sample t-test** was used to compare ticket prices between Business and Economy fare classes.

The purpose of the test was to determine whether the difference in average ticket prices between the two groups was statistically significant.

The analysis found a statistically significant difference between Business and Economy ticket prices.

### Aircraft Type Analysis

**ANOVA (Analysis of Variance)** was used to compare average ticket revenue across multiple aircraft types.

ANOVA was selected because the analysis involved more than two groups.

The results indicated statistically significant differences in average ticket revenue across aircraft types.

---

## Customer Segmentation

Customer segmentation was performed using **K-Means clustering**, an unsupervised machine learning algorithm.

The goal was to identify groups of customers with similar value and transaction characteristics without using predefined customer labels.

### Segmentation Process

1. Selected customer-level behavioral and value features
2. Prepared the features for modeling
3. Applied **StandardScaler** to place features on comparable scales
4. Tested multiple values of K
5. Evaluated clustering performance using the **Elbow Method** and **Silhouette Score**
6. Applied K-Means clustering
7. Compared the characteristics of the resulting customer groups

Scaling was important because K-Means is distance-based and the selected customer features had different numerical ranges.

The final analysis identified distinct customer groups with different customer-value and transaction characteristics.

---

## Key Insights

The analysis highlighted several important patterns:

- Customer spending varies significantly across the customer base.
- A relatively small group of customers represents substantially higher customer value.
- Revenue performance differs across airline routes.
- Economy generates the largest share of ticket volume, while Business class has a substantially higher average ticket value.
- Statistical testing confirmed meaningful differences in ticket prices between Business and Economy fare classes.
- Average ticket revenue also differs significantly across aircraft types.
- Customer segmentation identified groups with different value and transaction characteristics.

---

## Business Value

The analysis demonstrates how airline transactional data can support business decision-making in areas such as:

- **Customer segmentation** — identifying higher-value customer groups
- **Revenue analysis** — understanding major sources of airline revenue
- **Route performance** — identifying routes with stronger revenue contribution
- **Pricing analysis** — comparing ticket values across fare classes
- **Customer strategy** — supporting more targeted customer analysis and engagement
- **Operational analysis** — understanding differences across routes and aircraft types

These insights could help analysts and business teams prioritize areas for deeper investigation and support data-driven planning.

---

## Skills Demonstrated

This project demonstrates practical experience with:

- SQL joins and multi-table analysis
- CTEs and aggregations
- Relational data analysis
- Data validation and quality checks
- Exploratory Data Analysis (EDA)
- Customer and revenue analytics
- Statistical hypothesis testing
- K-Means clustering
- Feature scaling
- Model evaluation
- Data visualization
- Translating analytical results into business insights

---

## Project Structure

The Jupyter Notebook contains the complete analytical workflow, including:

- SQL queries
- Data validation
- Exploratory analysis
- Revenue analysis
- Statistical tests
- Customer segmentation
- Visualizations
- Business interpretations
