#  E2E Manual API Testing for E-commerce Project

This repository contains end-to-end manual API test cases for an e-commerce system. It includes authentication, product, and order management flows using **Postman** and is executed using **Newman** with detailed HTML reporting.

---

##  Test Scenarios Covered

-  **User Login**

  - Extracts `token` and `userId` from response.

-  **Add Product**

  - Add new product with multiple attributes to the website.

-  **Create Order**

  - Places order using product and user information.

-  **Get Order Details**

  - Retrieves details of the created order.

-  **Delete Order**

  - Deletes the created order by ID.

-  **Delete Product**
  - Removes the previously added product.

# 🛠 Setup Instructions

This guide helps you install the necessary tools and run the E2E manual API test collection for the E-commerce system.

---

## 🛠 Install Newman CLI Globally

```bash
npm install -g newman
npm install -g newman-reporter-html
```

## 🛠 Running the Tests

```bash
newman run Ecom.postman_collection.json \
  --iteration-data data.csv \
  --reporters cli,html \
  --reporter-html-export reports/ecom-report.html
```
