# Chapter 3

# Requirement Engineering

## 3.1 Requirement Analysis

Requirement analysis is an important stage in the development of the **Design and Development of a Web-Based E-Commerce Management System for Pure Haven BD** project. This stage helped identify the main needs of the system, the expected users, the required functions, and the operational behavior of the proposed e-commerce platform.

Pure Haven BD is designed as a web-based shopping and management system where customers or visitors can browse products, search and filter items, view product details, add products to the cart or wishlist, place orders, select a payment method, track orders, and send messages through the website. On the other side, the Admin can manage products, categories, subcategories, customer orders, customer messages, homepage promotional content, homepage slider content, footer settings, and site settings.

The requirement analysis focused on two major roles: **Customer/Visitor** and **Admin**. The Customer/Visitor side emphasizes product discovery, order placement, and user convenience. The Admin side emphasizes business management, product control, order processing, and content management. The system requirements were prepared according to the actual modules and confirmed features of the Pure Haven BD project.

The main purpose of the requirement analysis was to ensure that the system supports the core needs of an e-commerce platform while maintaining a simple, organized, and user-friendly workflow for both customer-side users and administrators.

## 3.2 Requirement Engineering

Requirement engineering defines, organizes, and documents what the system should do and how it should behave. For Pure Haven BD, the requirement engineering process was based on the confirmed features of the project, including product catalog management, cart and wishlist management, checkout, order tracking, admin dashboard, order management, customer message management, homepage content management, and site settings management.

The requirements are divided into user requirements, system requirements, functional requirements, non-functional requirements, hardware requirements, and software requirements.

### 3.2.1 User Requirements

The user requirements describe the expectations of the main users of the system. The Pure Haven BD system has two main roles: Customer/Visitor and Admin.

#### Customer/Visitor Requirements

The Customer/Visitor should be able to:

- Visit the homepage and view promotional sections, category sections, product sections, deals, and site information.
- Browse available products from the shop page.
- Search products using keywords.
- Filter products based on category and subcategory.
- View product details, including image, name, price, description, stock-related information, and available variants.
- Add selected products to the shopping cart.
- Update product quantity in the cart.
- Remove products from the cart.
- Add preferred products to the wishlist.
- Remove products from the wishlist.
- Proceed to checkout from the cart.
- Provide necessary customer and delivery information during checkout.
- Select a payment method from Cash on Delivery, bKash, and Nagad.
- Place an order successfully.
- View order success confirmation after placing an order.
- Track order status using order-related information.
- Send messages or contact requests through the website.
- View static information pages such as contact, offers, privacy policy, and terms and conditions.

#### Admin Requirements

The Admin should be able to:

- Access the admin panel through admin login.
- View the admin dashboard with important business summaries.
- Add new products with product information, image, price, category, stock, and variant-related details.
- Edit existing product information.
- Delete products when required.
- Manage product categories and subcategories.
- View customer orders.
- Search, filter, and manage orders.
- Update order status based on business processing needs.
- View printable order voucher or invoice-style order information.
- View customer messages.
- Manage customer message status or response-related information.
- Manage homepage promotional content.
- Manage homepage slider content.
- Manage footer-related settings.
- Manage site branding and site settings.

### 3.2.2 System Requirements

System requirements describe the services and operations that the Pure Haven BD system must provide to support both Customer/Visitor and Admin activities.

#### Customer/Visitor Side System Requirements

The system should:

- Display a clean and organized homepage for visitors.
- Show product listings with product name, image, price, and category information.
- Allow product search and filtering.
- Display detailed product information on a separate product details page.
- Maintain cart data during the shopping process.
- Maintain wishlist data for selected products.
- Calculate cart totals correctly based on product price and quantity.
- Allow checkout using customer and delivery information.
- Support payment method selection for Cash on Delivery, bKash, and Nagad.
- Store order information after checkout.
- Display an order success page after successful order submission.
- Allow customers or visitors to track order status.
- Store customer messages submitted through the website.

#### Admin Side System Requirements

The system should:

- Provide an admin login system for admin panel access.
- Display dashboard summaries for administrative monitoring.
- Allow product creation, editing, deletion, and listing.
- Allow product image upload during product management.
- Allow category and subcategory management.
- Allow admin to view, filter, and update orders.
- Allow admin to view order details and voucher-style order information.
- Allow admin to manage customer messages.
- Allow admin to manage homepage promotional content.
- Allow admin to manage homepage slider content.
- Allow admin to manage footer and site settings.
- Store and retrieve product, order, category, subcategory, slider, message, and settings data properly.

### 3.2.3 Functional Requirements

Functional requirements define the specific operations that the system must perform. The confirmed functional requirements of Pure Haven BD are listed below.

#### Product and Catalog Functions

- The system shall display product lists on the shop page.
- The system shall display individual product details.
- The system shall allow product search by keyword.
- The system shall allow product filtering by category and subcategory.
- The system shall support product variants where applicable.
- The system shall show product price, image, category, and description.

#### Cart and Wishlist Functions

- The system shall allow Customer/Visitor to add products to the cart.
- The system shall allow Customer/Visitor to update product quantity in the cart.
- The system shall allow Customer/Visitor to remove products from the cart.
- The system shall calculate total price based on selected products and quantities.
- The system shall allow Customer/Visitor to add products to the wishlist.
- The system shall allow Customer/Visitor to remove products from the wishlist.

#### Checkout and Order Functions

- The system shall allow Customer/Visitor to proceed from cart to checkout.
- The system shall collect customer name, phone, address, and required order information.
- The system shall allow Customer/Visitor to select Cash on Delivery, bKash, or Nagad as the payment method.
- The system shall create an order after checkout submission.
- The system shall display an order success confirmation.
- The system shall allow Customer/Visitor to track order status.

#### Admin Product Management Functions

- The system shall allow Admin to add new products.
- The system shall allow Admin to edit existing products.
- The system shall allow Admin to delete products.
- The system shall allow Admin to upload product images.
- The system shall allow Admin to manage stock-related product information.
- The system shall allow Admin to manage product variants.

#### Admin Category Management Functions

- The system shall allow Admin to create categories.
- The system shall allow Admin to edit categories.
- The system shall allow Admin to delete categories.
- The system shall allow Admin to manage subcategories connected with categories.

#### Admin Order Management Functions

- The system shall allow Admin to view customer orders.
- The system shall allow Admin to search or filter orders.
- The system shall allow Admin to update order status.
- The system shall allow Admin to view order voucher or invoice-style information.

#### Message and Content Management Functions

- The system shall allow Customer/Visitor to submit messages.
- The system shall allow Admin to view and manage customer messages.
- The system shall allow Admin to manage homepage promotional content.
- The system shall allow Admin to manage homepage slider content.
- The system shall allow Admin to manage footer settings.
- The system shall allow Admin to manage site settings and branding-related information.

### 3.2.4 Non-Functional Requirements

Non-functional requirements define the quality, usability, and performance expectations of the system.

#### Usability

- The system should provide a simple and understandable interface for Customer/Visitor and Admin.
- Product browsing, cart management, checkout, and order tracking should be easy to use.
- Admin pages should be organized so that products, categories, orders, messages, and settings can be managed efficiently.

#### Performance

- The system should load product pages, shop pages, and admin pages within an acceptable response time.
- Cart, wishlist, filtering, and order-related operations should work smoothly during normal use.

#### Reliability

- The system should store product, order, category, message, and settings data correctly.
- The system should maintain order information after checkout.
- Admin changes should be reflected properly in the relevant website sections.

#### Maintainability

- The system should be structured in a modular way so that future improvements can be added without changing the entire system.
- Separate modules for products, categories, orders, messages, homepage content, and settings support better maintenance.

#### Compatibility

- The system should work on modern web browsers.
- The website should be accessible from desktop and mobile devices through responsive interface design.

#### Security and Access Control

- Admin-side functions should be accessible through the admin login system.
- Customer order information and message information should be handled responsibly within the system.

### 3.2.5 Hardware Requirements

The exact processor and RAM specification used during development is not available. However, based on the nature of the project, the required hardware categories are listed below.

| Hardware Component | Requirement |
| --- | --- |
| Development computer | A laptop or desktop capable of running a modern web development environment |
| Processor | [not available] |
| RAM | [not available] |
| Storage | Sufficient storage space for project source code, dependencies, product images, database-related files, and documentation |
| Internet connection | Stable internet connection for package installation, testing, development support, and accessing web-based resources |
| Client device | Desktop, laptop, tablet, or smartphone with a modern web browser |
| Server/hosting environment | A hosting environment capable of running a Next.js web application and connecting with a PostgreSQL database |

### 3.2.6 Software Requirements

The software requirements are based on the confirmed technology stack of the Pure Haven BD project.

| Software Component | Requirement |
| --- | --- |
| Operating system | [not available] |
| Frontend framework | Next.js App Router with React |
| Programming language | TypeScript |
| Styling framework | Tailwind CSS with custom global CSS |
| Backend/API | Next.js API Route Handlers |
| Database | PostgreSQL |
| ORM | Prisma ORM |
| Package manager | npm or equivalent JavaScript package manager |
| Code editor | Visual Studio Code or equivalent editor |
| Web browser | Modern browser such as Chrome, Edge, Firefox, or equivalent |
| Image/file handling | Local product image upload folder |
| Additional storage | JSON files for selected settings, promotional content, messages, and admin-related settings |

## 3.3 Use Case Diagram of the System

The use case diagram represents the interaction between the main users and the Pure Haven BD system. It shows how Customer/Visitor and Admin actors use different system functions. The diagram helps to understand the system boundary, user responsibilities, and major functional areas of the e-commerce management system.

### 3.3.1 Use Case Symbol Table

| Symbol Name | Meaning |
| --- | --- |
| Actor | Represents an external user or role that interacts with the system, such as Customer/Visitor or Admin |
| Use Case | Represents a function or service provided by the system, such as Browse Products, Add to Cart, Place Order, or Manage Products |
| System Boundary | Represents the Pure Haven BD system and separates internal system functions from external actors |
| Association | Shows communication between an actor and a use case |
| Include Relationship | Shows that one use case always uses another use case as part of its process |
| Extend Relationship | Shows an optional or conditional function that may extend another use case |

### 3.3.2 Use Case Diagram Placement

**Figure 3.1 Use Case Diagram of Pure Haven BD**

The diagram will be placed below this caption in the final report.

The use case diagram should contain two main actors: **Customer/Visitor** and **Admin**. The Customer/Visitor side should include use cases such as Browse Products, Search/Filter Products, View Product Details, Add to Cart, Manage Wishlist, Checkout, Select Payment Method, Place Order, Track Order, and Send Message. The Admin side should include Login, Manage Products, Manage Categories, Manage Orders, Manage Customer Messages, Manage Homepage Promotional Content, Manage Home Slider, Manage Footer Settings, and Manage Site Settings.

### 3.3.3 Use Case Diagram Description

The use case diagram of Pure Haven BD shows the functional relationship between system users and the e-commerce platform. The Customer/Visitor interacts with the public side of the website. This actor can browse the homepage, search and filter products, view product details, add products to the cart, save products to the wishlist, proceed to checkout, select a payment method, place an order, track order status, and submit messages.

The Admin interacts with the management side of the system. After accessing the admin panel, the Admin can manage products, categories, subcategories, orders, customer messages, promotional content, home slider content, footer settings, and site settings. The Admin is responsible for maintaining the product catalog, processing customer orders, updating content, and keeping the website information organized.

The diagram should show the Pure Haven BD system as the central system boundary. The Customer/Visitor actor should be placed on one side and connected to customer-facing use cases. The Admin actor should be placed on the other side and connected to admin-facing use cases. This structure will clearly represent how the system supports both online shopping activities and e-commerce management activities.
