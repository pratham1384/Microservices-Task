# Microservices Containerization with Node.js, Docker, and Docker Compose

## 🧠 Overview
This project containerizes three Node.js microservices — **User**, **Product**, **Orders** and **Gateway** — and orchestrates them with Docker Compose.

## 🏗️ Services
| Service | Port | Description |
|----------|------|-------------|
| user-service | 3000 | Handles user data |
| product-service | 3001 | Manages product information |
| order-service | 3002 | Manages order data 
| gateway-service | 3003 | Acts as API gateway |

File structure

submission/
├── user-service/
│   └── app.js
│   └── package.json
│   └── Dockerfile
│
├── product-service/
│   └── app.js
│   └── package.json
│   └── Dockerfile
│
├── order-service/
│   └── app.js
│   └── package.json
│   └── Dockerfile
│
├── gateway-service/
│   └── app.js
│   └── package.json
│   └── Dockerfile
│
├── docker-compose.yml
└── README.md

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone <your-forked-repo-url>
<img width="940" height="223" alt="image" src="https://github.com/user-attachments/assets/74d37ee8-4b44-4ce9-bc6f-05c393c5646e" />


2. Build the Containers
docker-compose build

<img width="940" height="223" alt="image" src="https://github.com/user-attachments/assets/bef3368e-6c63-4c7b-be09-0aee3175470f" />
<img width="940" height="273" alt="image" src="https://github.com/user-attachments/assets/08c72991-2266-4a48-9dce-7626d56c0501" />


3. Run the Services
docker-compose up
<img width="940" height="347" alt="image" src="https://github.com/user-attachments/assets/730ae80c-6866-4e5f-9849-9e09f2687340" />

4. Verify Services
   
Visit:
<img width="940" height="245" alt="image" src="https://github.com/user-attachments/assets/6f1246dc-9977-4330-84aa-d7d3c7144099" />

User Service → http://localhost:3000/users
<img width="940" height="245" alt="image" src="https://github.com/user-attachments/assets/e8214b31-004f-486f-bf6f-ade5719aeab6" />

Product Service → http://localhost:3001/products
<img width="940" height="455" alt="image" src="https://github.com/user-attachments/assets/56cfd374-85c4-4b8e-9715-97cfb4c0df09" />

Order Service → http://localhost:3002/orders
<img width="940" height="360" alt="image" src="https://github.com/user-attachments/assets/7fb40700-5599-40f6-986d-a0d6c417992d" />

Gateway Service →
http://localhost:3003/api/users
<img width="940" height="265" alt="image" src="https://github.com/user-attachments/assets/ebeac1a7-9847-48ab-bf68-bd21393b82f8" />

http://localhost:3003/api/products
<img width="940" height="230" alt="image" src="https://github.com/user-attachments/assets/653661a8-cccd-4e24-addf-fd1aeb5ac799" />

http://localhost:3002/api/orders
<img width="980" height="229" alt="image" src="https://github.com/user-attachments/assets/e6cc7830-8064-4b92-817f-a6bb18da269c" />

									
				
🧪 Testing Each Service

Use curl or browser to confirm responses:

curl http://localhost:3000/users
<img width="940" height="440" alt="image" src="https://github.com/user-attachments/assets/874936e7-97d8-445e-854e-1e2551be9938" />

curl http://localhost:3001/products
<img width="940" height="438" alt="image" src="https://github.com/user-attachments/assets/1b1af1ba-21a7-4d05-9708-a2cd4d189449" />

curl http://localhost:3002
<img width="940" height="430" alt="image" src="https://github.com/user-attachments/assets/a9532330-b0ae-4828-8442-4906a8e272a3" />



