# Project Overview
Implementation of a **CRUD system** based on a **REST API** (**Representational State Transfer Application Programming Interface**) using standard **HTTP** methods (**GET/POST/PUT/DELETE**) on a local **XAMPP** server (**Apache**), including search and pagination functionality.

I also implemented protection against **Cross-Site Scripting (XSS)** attacks using PHP functions such as **`htmlspecialchars()`** and **`strip_tags()`**.

The project follows a **client-server architecture**, where the user sends different **requests**, and receives HTTP response codes via **`http_response_code()`**, such as:
* 200 – OK  
* 201 – Created (used with POST)  
* 400 – Bad Request (missing required parameters)  
* 401 – Unauthorized (missing authentication parameters)  
* 403 – Forbidden (authenticated but lacking required permissions)  
* 404 – Not Found, etc.

The server (API) responds with a status code and valid **JSON (JavaScript Object Notation)**, returning raw data using **`json_encode()`** and **`json_decode()`**.

I also used the **PDO (PHP Data Objects)** extension, which provides a universal interface for accessing different databases with various **SQL** dialects.

Within SQL queries, I utilized clauses such as:
**SELECT**, **LEFT JOIN**, **ORDER BY (DESC)**, **INSERT INTO**, **WHERE**, **LIMIT**, **UPDATE SET**, **DELETE**, and **LIKE** (for keyword-based search).

Initially, I created the database (named *autosalon_api*) using the web interface **PhpMyAdmin**, performing some initial manual configurations.

Afterward, I executed SQL queries of type **INSERT INTO VALUES** to automatically populate the previously created tables with sample data, avoiding time-consuming manual input.

![screen1](screenshots/Screenshot_1.jpg)
![screen2](screenshots/Screenshot_2.jpg)
![screen3](screenshots/Screenshot_3.jpg)
![screen4](screenshots/Screenshot_4.jpg)

# Functionality Testing (Postman)
Below are screenshots demonstrating REST API testing performed using **Postman**, a tool I also had the opportunity to use during my internship at Unifun.

![screen5](screenshots/Screenshot_5.jpg)
![screen6](screenshots/Screenshot_6.jpg)
![screen7](screenshots/Screenshot_7.jpg)
![screen8](screenshots/Screenshot_8.jpg)
![screen9](screenshots/Screenshot_9.jpg)
![screen10](screenshots/Screenshot_10.jpg)
![screen11](screenshots/Screenshot_11.jpg)
![screen12](screenshots/Screenshot_12.jpg)
![screen13](screenshots/Screenshot_13.jpg)
![screen14](screenshots/Screenshot_14.jpg)
