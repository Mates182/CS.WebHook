# Webhook Example in ASP.NET 8 - C#

This project is a simple implementation of a Webhook in ASP.NET 8, designed to receive and process POST requests with a JSON payload.

## 🛠 Features

- Built with **ASP.NET 8**.
- Simple and clean architecture for handling webhook requests.
- Acknowledgment of the received webhook with a 200 HTTP status code.

## 🚀 Getting Started

### Prerequisites

- **Visual Studio Community 2022** (recommended)  
- .NET 8 SDK  

### 🔧 Installation Steps

1. Clone the repository:  
   ```bash
   git clone https://github.com/Mates182/CS.WebHook.git
   ```
   ```bash
   cd CS.WebHook
   ```

2. Open the project in **Visual Studio Community 2022**.  

3. Run the application using the Visual Studio debugger or the command:  
   ```bash
   dotnet run
   ```

4. The application will start on `https://localhost:7286`.

## 🌐 How to Test

You can test the Webhook using **Postman** or any HTTP client.  

### Example Request

- **URL**: `https://localhost:7286/webhook`  
- **Method**: POST  
- **Headers**:  
  - `Content-Type`: application/json  
- **Body** (raw, JSON):  
  ```json
  {
    "Header": "Header",
    "Body": "Hello Webhook :D"
  }
  ```

### Expected Response

- **Status Code**: `200 OK`  
- **Response Body**:  
  ```
  Webhook Ack!
  ```

### Console Output

On receiving a request, the following will be logged to the console:  
```
Header: Header, Body: Hello Webhook :D
```
