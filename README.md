# Customer Purchase analyze

##  Objective
This project will show how to analyze customer purchase data stored in a database using both:
1) SQL queries
2) Python with Pandas


## Scenario
We want to analyze total item purchases by customers aged (18–35). 

## Database Structure
The database consists of four tables:
- **Customer** (`customer_id`, `age`)
- **Sales** (`sales_id`, `customer_id`)
- **Orders** (`order_id`, `sales_id`, `item_id`, `quantity`)
- **Items** (`item_id`, `item_name`)

## **Relationships:**
- One customer can make many sales
- One sale can include multiple orders (items)
- Quantity may be `NULL` or `0` (indicating no purchase)
---

## Goal
Generating CSV report for customers aged (18–35) showing:
- Total quantity bought for each item
- Only items with quantity > 0
- No decimal values
- Output format with `;` as the delimiter:
