![image](https://github.com/user-attachments/assets/58803112-f914-416f-bf88-9f182d80c60e)
![image](https://github.com/user-attachments/assets/7427892b-d795-4a0e-bc19-142427bcffbb)
![image](https://github.com/user-attachments/assets/b4d90b06-212d-4c5b-bf63-5ba23ca93e42)
![image](https://github.com/user-attachments/assets/8b3b63d0-ecca-4698-806f-c59087320e14)
![image](https://github.com/user-attachments/assets/cbd31b76-129e-4738-801d-455af344e195)
![image](https://github.com/user-attachments/assets/43aab02d-994c-48bf-bf22-0dc656704863)
![image](https://github.com/user-attachments/assets/4f59fad8-8d19-4734-98c6-e6bd4d8d8c84)
![image](https://github.com/user-attachments/assets/8c568ff9-c81e-47e5-addf-deb3710fe2ed)
![image](https://github.com/user-attachments/assets/2634b60c-324f-4eb4-ace8-8ac93e4830f8)
![image](https://github.com/user-attachments/assets/9b0a3201-2ab3-4156-af27-8a0b417ea812)
![image](https://github.com/user-attachments/assets/ee1bcd64-7e7e-4588-ba5d-70507fe9d9fa)
![image](https://github.com/user-attachments/assets/8fc85656-9f85-47d5-be05-70c5a8653751)













Pharmveda

User Role: Customer

Permissions:
Search for medicines: Customers can search for medications by name or category using a search bar or filter options, making it easy to find products.
Add medicines to the cart: Customers can add medications to their shopping cart, allowing them to review and modify their selections before checkout.
Proceed to checkout with flexible payment options: After selecting items, users can proceed to a secure checkout, where they can choose from different payment methods (credit/debit card, online wallets, etc.).
Track order status in real time: Once the order is placed, customers can track their order's status in real-time, such as "Processing," "Shipped," or "Delivered."
Cancel orders if applicable: If the order hasn't been processed or shipped yet, customers can cancel it through their dashboard.

Restricted Actions:
Cannot manage stock or view inventory data: Customers cannot access the admin tools for managing product inventory levels, ensuring that sensitive backend operations remain restricted.
No access to other users' data or admin features: Customers cannot view other users’ order history, personal data, or interact with admin functionalities like adding products or managing sales.

User Role: Admin

Permissions:
View real-time stock levels and inventory data: Admins have full access to inventory management, including the ability to view current stock levels for each product in real time.
Monitor usage patterns for medications: Admins can track which products are frequently ordered, identifying sales trends and demand patterns to optimize stock management.
Add or update stock levels as required: Admins can add new stock or update existing stock quantities, ensuring the platform always reflects accurate availability.
Manage all orders, including processing, tracking, and cancellations: Admins can view and manage all customer orders, including fulfilling orders, updating order status, and handling cancellations.

Restricted Actions:
No access to the customer’s personal order history (beyond admin duties): While admins can view orders for processing purposes, they cannot access detailed customer data beyond the order and shipping details.

Technical Implementation in MERN Stack

Authentication:

JWT Tokens: During login, a JWT (JSON Web Token) is generated, which contains the user’s role (either customer or admin). The token is signed and stored in an HTTP-only cookie or local storage, ensuring secure identification of the user.
The token is sent in the Authorization header for each subsequent request, allowing the server to verify the user's identity.

Authorization:
Middleware for Role Verification: Custom middleware checks the user's role and verifies whether they have the necessary permissions to access specific API routes.
For example, the /inventory route will only be accessible to users with the admin role.
Middleware checks the JWT token on each request to ensure the user has the right role and hasn't been logged out or their token expired.


Frontend  And UI :
The Pharmveda UI is designed for simplicity and a smooth user experience. On the frontend, I used React to create interactive components, including a search bar for medicines, a cart system for easy item management, and a checkout process with multiple payment options. Admin functionalities are incorporated in a secure dashboard where admins can manage stock, track sales, and process orders. The layout is responsive, ensuring compatibility across devices, and  CSS is used for styling to ensure a modern and consistent design.

Repository : https://github.com/Avanisrepositories/Pharmveda.git












