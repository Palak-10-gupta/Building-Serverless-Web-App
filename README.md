# ⚡ Serverless Registration Web App – AWS

This project demonstrates a **serverless web application** for user registration using **AWS Lambda, DynamoDB, and API Gateway**.  
It highlights creating a fully functional, scalable, and cost-effective serverless architecture.

<p align="center">
  <img src="https://github.com/user-attachments/assets/90fbefae-0c5a-42bd-87c0-2c1735547748" alt="Architecture Diagram" width="1280" height="720" />
</p>

---

## 🛠️ Tech Stack
- **Backend:** AWS Lambda, API Gateway  
- **Database:** DynamoDB  
- **Access Control:** IAM Roles  
- **Other Tools:** CloudWatch for monitoring  

---

## 🛠️ Steps to Build the Project

### 1️⃣ Step 1: Create a DynamoDB Table

- **Table Name:** `registration-table`  
- **Purpose:** Store registered user data securely.

---

### 2️⃣ Step 2: Create IAM Role for Lambda

- **Role Name:** `RegistrationRoleForm`  
- **Permissions Required:**  
  1. CloudWatch Full Access  
  2. DynamoDB Full Access  

---

### 3️⃣ Step 3: Create Lambda Function

- **Function Name:** `registration-form-function`  
- **Purpose:** Handle user registration logic.

---

### 4️⃣ Step 4: Write Lambda Function ✍️

- **API Endpoint Update:**  
```javascript
// Replace this
'https://r3u6mpiyr2.execute-api.ap-south-1.amazonaws.com/prod'
// With this
'API_URL/register'

```

### 5️⃣ Step 5: Create and deploy API Gateway 🌐

- **Deploy Lambda via API Gateway:**  
  Use **API Gateway** to deploy your Lambda function as a REST API endpoint.

- **Enable CORS:**  
  Configure the API Gateway to allow cross-origin requests from your frontend.

**CORS Configuration:**  
```text
Access-Control-Allow-Origin: '*'
Access-Control-Allow-Headers: Content-Type,X-Amz-Date,Authorization,X-Api-Key,X-Amz-Security-Token
Access-Control-Allow-Methods: POST
```

### 6️⃣ Step 6: Test the project.Registration is successful ✅

- **Access the Web App:**  
  Open the frontend application in your browser and register a user.

- **Verify Registration:**  
  Ensure that the registration is successful and that the user data is correctly stored in **DynamoDB**.

- **Check CORS:**  
  Confirm that **API Gateway CORS settings** allow requests from your frontend, enabling smooth communication between client and server.

## 📸 Screenshots

<p align="center">
  <img src="https://raw.githubusercontent.com/Palak-10-gupta/Building-Serverless-Web-App/main/enterdetails.png" alt="Enter Details" width="600" />
  <img src="https://raw.githubusercontent.com/Palak-10-gupta/Building-Serverless-Web-App/main/registrationfailed.png" alt="Registration Failed" width="600" />
  <img src="https://raw.githubusercontent.com/Palak-10-gupta/Building-Serverless-Web-App/main/registrationform.png" alt="Registration Form" width="600" />
  <img src="https://raw.githubusercontent.com/Palak-10-gupta/Building-Serverless-Web-App/main/registrationsuccessful.png" alt="Registration Successful" width="600" />
</p>

---

## 👨‍💻 Author
**Palak Gupta**  
💼 GitHub: [@Palak-10-gupta](https://github.com/Palak-10-gupta)

---

⭐ If you like this project, don’t forget to give it a **star** on GitHub! ⭐


