# Ecomerce
Django Ecommerce API 

# Ecommerce Hoodie App
Welcome to our Ecommerce Hoodie App! This project aims to provide a seamless shopping experience for hoodie enthusiasts. Here's an overview of the features and functionality:

# Homepage
The homepage showcases a variety of hoodie products available for purchase.
Clients can easily navigate through the products and explore different categories.
# Search Bar
Clients can use the search bar to find specific hoodie products based on their preferences.
The search functionality makes it convenient for users to find their desired items quickly.
# About Section
The About section provides information about the Ecommerce Hoodie App, including its mission and values.
Clients can learn more about the app and its creators.
# Login Page
Users have the option to log in to their accounts to access personalized features and preferences.
Secure authentication ensures user data privacy and security.
# Register Page
New users can register for an account to unlock additional features and benefits.
Registration is quick and easy, allowing users to create their profiles seamlessly.
# Profile Page
The Profile page allows users to view and update their user details, such as name, email, password, and additional information like address, contact details, etc.
Users can update their information as needed, ensuring their profiles are accurate and up to date.
# User Info Page
The User Info page allows users to provide additional details about themselves, such as address, contact information, and other relevant information.
Users can add or update their information as needed, ensuring a personalized and tailored experience.
# Product Categories Page
The Product Categories page organizes hoodie products into different categories for easy browsing.
Two main categories are available: Special Hoodies and Common Hoodies.
Each category has its own dropdown page, showcasing hoodies belonging to the respective category.
# Product Details Page
When a user clicks on a specific hoodie product, they are directed to the Product Details page.
Here, users can view detailed information about the hoodie, including its price, description, and images.
Users have the option to select the quantity of the hoodie they wish to purchase and add it to their cart.
# Cart Page
The Cart page displays all the hoodie products that users have added to their shopping cart.
Users can review their selected items, adjust quantities, and remove items from their cart.
Once satisfied with their selection, users can proceed to checkout.
# Checkout Process
The checkout process allows users to finalize their purchases and process their payments.
Secure payment integration ensures safe and seamless transactions for users.
Users can review their order details, enter shipping and billing information, and complete their purchase.

# Introduction
Our Ecommerce Hoodie App is a Django-based web application designed to offer a seamless shopping experience for hoodie enthusiasts. The app allows users to browse a variety of hoodie products, search for specific items, create accounts, and manage their profiles. With secure authentication and payment integration, users can easily purchase their favorite hoodies and enjoy a convenient shopping experience.

# Features
Homepage showcasing hoodie products
Search bar for finding specific products
About section providing app information
User authentication (login and registration)
Profile page for updating user details
Product categories page with dropdown categories
Product details page with quantity selection
Cart page for managing selected items
Checkout process for finalizing purchase
Setup Instructions

* To set up the Ecommerce Hoodie App locally, follow these steps: 

# Clone the repository to your local machine:


git clone <repository-url>

# Navigate to the project directory:


cd ecommerce-hoodie-app
# Create a virtual environment and activate it:


python -m venv env
source env/bin/activate
# Install dependencies from the requirements.txt file:


pip install -r requirements.txt
# Apply migrations to create the database schema:


python manage.py migrate
# Run the development server:


python manage.py runserver

Access the app in your web browser at http://127.0.0.1:8080/.


# Once the app is set up and running, users can:

Browse hoodie products on the homepage
Use the search bar to find specific products
View detailed information about products on the product details page
Add products to the cart and manage selected items
Proceed to checkout to finalize purchases
Register for an account and log in to access personalized features
Update user details and profile information on the profile page
Explore different product categories and view related products



# Endpoints

- Homepage
URL: /
Method: GET
Description: Displays the homepage with hoodie products.
- About Section
URL: /about/
Method: GET
Description: Displays information about the app.
- Login Page
URL: /login/
Method: GET, POST
Description: Allows users to log in to their accounts.
- Logout Page
URL: /logout/
Method: GET
Description: Allows users to log out of their accounts.
- Register Page
URL: /register/
Method: GET, POST
Description: Allows new users to register for an account.
- Profile Page
URL: /update_user/
Method: GET, POST
Description: Allows users to view and update their user details.
- User Info Page
URL: /update_info/
Method: GET, POST
Description: Allows users to add additional details about themselves.
- Product Categories Page
URL: /category/<str:foo>/
Method: GET
Description: Displays hoodie products belonging to a specific category.
- Product Details Page
URL: /product/<int:pk>/
Method: GET
Description: Displays detailed information about a specific hoodie product.
- Cart Page
URL: /cart/
Method: GET
Description: Displays all hoodie products added to the shopping cart.
- Search Page
URL: /search/
Method: GET, POST
Description: Allows users to search for specific hoodie products.

# Request/Response Formats

Request Methods: GET, POST
Response Formats: HTML pages rendered using Django templates
# Authentication: User authentication using Django's built-in authentication system
Authentication Methods
User authentication is handled using Django's built-in authentication system. Users can log in to their accounts using their username and password. New users can register for an account to access additional features.

# Usage Examples
- Example 1: Registering for an Account
Navigate to the Register page (/register/).
Fill out the registration form with your desired username and password.
Click the "Register" button to submit the form.
Upon successful registration, you will be redirected to the Profile page (/update_info/) to add additional details about yourself.
- Example 2: Logging In to Your Account
Navigate to the Login page (/login/).
Enter your username and password.
Click the "Login" button to log in to your account.
Upon successful login, you will be redirected to the Homepage (/) to start browsing hoodie products.
- Example 3: Viewing and Updating User Details
Navigate to the Profile page (/update_user/).
View your current user details.
Update your user details as needed.
Click the "Save" button to save your changes.
- Example 4: Adding Additional User Info
Navigate to the User Info page (/update_info/).
Fill out the form with additional details about yourself, such as address and contact information.
Click the "Save" button to save your changes.