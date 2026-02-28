Ticket Booking Microservices System

A distributed Spring Boot microservices application demonstrating scalable backend architecture using event-driven communication, authentication, and API gateway routing.

📌 Project Overview
This project is based on the original work by Leetjourney and is licensed under CC BY-NC 4.0.
Significant modifications and extensions were implemented to enhance functionality, architecture reliability, and security.

✨ My Contributions
Refactored service configurations
Fixed Kafka broker connection issues
Added secure authentication flow with Keycloak
Improved inter-service communication
Updated application properties and environment configs
Enhanced error handling and stability

🏗️ Architecture
The system follows a microservices architecture with independent services communicating via REST and Kafka events.
Services included:
API Gateway → Request routing & security
Booking Service → Handles ticket booking logic
Order Service → Processes orders asynchronously
Inventory Service → Manages event & seat data
Keycloak → Authentication & authorization
Kafka → Event streaming

⚙️ Tech Stack
Java + Spring Boot
Spring Cloud Gateway
Apache Kafka
Keycloak
MySQL
Docker
Maven

🔁 Workflow
Client sends request → API Gateway
Gateway authenticates via Keycloak
Booking Service validates request
Event sent to Kafka
Order Service consumes event
Inventory Service updates availability

🚀 How to Run
# start infrastructure
docker compose up -d

# run services
run InventoryService
run BookingService
run OrderService
run ApiGateway

🎯 Learning Outcomes
This project demonstrates practical understanding of:
Distributed systems design
Event-driven architecture
Secure authentication in microservices
Service orchestration
Debugging real-world service communication issues

📜 License

This project is adapted from:
Leetjourney — Spring Boot Microservices/ https://github.com/leetjourney/leetjourney-spring-boot-microservices
Licensed under Creative Commons BY-NC 4.0

You may:
Share
Modify
Learn from it

You may NOT use it commercially.
