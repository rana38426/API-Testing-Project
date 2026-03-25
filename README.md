# 🧪 API Testing Project (Postman)

## 📌 Project Overview

This project demonstrates end-to-end API testing using Postman on the FakeStore API. It covers functional, negative, and validation testing along with real defect identification.

---

## 🛠️ Tools & Technologies

* Postman (API Testing)
* JavaScript (Postman Test Scripts)
* GitHub (Version Control)

---

## 📂 Project Structure

* **Postman_Collection.json** → Contains all API requests and test scripts
* **FakeStore_Environment.json** → Stores environment variables (base_url, product_id)
* **TestCases.xlsx** → Detailed test scenarios and expected results
* **README.md** → Project documentation

---

## ✅ Test Coverage

### 🔹 GET APIs

* Get all products
* Get single product (valid & invalid ID)
* Invalid endpoint
* Response time validation
* Response structure validation
* Content-Type validation
* Unauthorized access

### 🔹 POST APIs

* Create product (valid data)
* Create product (missing fields)
* Create product (empty body)
* Create product (invalid data types)
* Create product (large input data)

### 🔹 PUT APIs

* Update product (valid ID)
* Update product (invalid ID)

### 🔹 DELETE APIs

* Method not allowed validation

---

## 🔍 Key Validations Performed

* Status code validation
* Response time check
* Response structure & schema validation
* Header validation
* Data type validation
* Negative testing (invalid inputs, wrong methods)
* Data consistency testing (POST → GET)

---

## ⚠️ Defects Identified

* Invalid product ID returns **200 instead of 404**
* API allows access without authentication (**no 401 response**)
* API accepts invalid data types without validation
* Data is not persisted after POST request

---

## 🔁 API Chaining Example

* Created product using POST
* Stored product ID using environment variables
* Fetched same product using GET
* Validated response data consistency

---

## ▶️ How to Run the Project

1. Open Postman
2. Import **Postman_Collection.json**
3. Import **FakeStore_Environment.json**
4. Select environment
5. Run requests manually OR use Collection Runner

---

## 🎯 Learning Outcomes

* Hands-on API testing using Postman
* Writing JavaScript test scripts
* Performing negative and edge-case testing
* Identifying and reporting API defects
* Using environment variables and API chaining

---

## 👨‍💻 Author

**Sudhir Rana**
