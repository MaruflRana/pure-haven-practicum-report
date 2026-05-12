Chapter 4

Analysis

4.1 Software Analysis Pattern

The Pure Haven BD system follows a layered web application analysis pattern. This pattern separates the system into different logical layers so that each part of the application can perform a specific responsibility. In this project, the public website, admin panel, API operations, data access mechanism, and data storage system are considered as separate but connected parts of the overall system.

The layered pattern is suitable for this project because Pure Haven BD includes both customer-facing functions and admin-side management functions. Customer/Visitor users interact with the public website to browse products, manage cart and wishlist items, place orders, select a payment method, track orders, and send messages. The Admin uses the management section to control products, categories, orders, homepage content, customer messages, footer settings, and site settings. By analyzing the system in layers, the project becomes easier to understand, document, maintain, and improve.

Presentation Layer

The presentation layer represents the user-facing part of the Pure Haven BD system. It includes the public website pages, admin panel pages, and reusable user interface components. Public pages include the homepage, shop page, product details page, cart page, wishlist page, checkout page, order success page, order tracking page, contact page, offers page, privacy policy page, and terms and conditions page. Admin pages include the dashboard and management pages for products, categories, orders, messages, homepage promotional content, home slider, footer settings, site settings, and admin settings.

Reusable UI components support consistency across the system. Components such as navigation, product cards, cart interface, wishlist interface, footer, home sections, and admin interface elements help keep the design organized and reduce repeated work. This layer is responsible for presenting information clearly and collecting input from Customer/Visitor and Admin users.

Application/API Layer

The application/API layer handles the functional processing of the system. In Pure Haven BD, this layer is represented by Next.js API route handlers. These API routes manage the communication between the user interface and the data layer. Major API operations include product management, order processing, category management, product image upload, customer message handling, homepage promotional content management, footer settings, site settings, and home slider management.

This layer receives user requests from the presentation layer, applies the required operation, and sends the appropriate response. For example, when a Customer/Visitor places an order, the checkout interface sends the order information to the order API. Similarly, when an Admin adds or edits a product, the admin product management page sends the product information to the product API.

Data Access Layer

The data access layer is responsible for structured communication with the database. In this project, Prisma ORM is used for structured data access. Prisma helps the system interact with database models such as Product, ProductVariant, Order, OrderItem, Category, Subcategory, and HomeSlide.

This layer improves the organization of database operations by allowing the application to create, read, update, and delete information in a structured way. Instead of mixing database operations directly into the user interface, the project keeps data-related activities behind the API and data access structure.

Data Storage Layer

The data storage layer stores the information required by the Pure Haven BD system. PostgreSQL is used for product, order, category, subcategory, order item, product variant, and homepage slider-related data. JSON-based storage is used for selected settings, customer messages, footer settings, admin settings, and promotional content. Browser localStorage is used for cart and wishlist data on the customer side.

This storage arrangement supports the main business operations of the system. Product and order-related data are stored in structured database form, while selected content and setting-related information are managed through JSON-based storage. Cart and wishlist information are maintained in the browser during customer-side interaction.

4.1.1 Reason for Choosing the Pattern

The layered web application analysis pattern was chosen because it supports a clear separation of responsibilities. Each layer has its own role, which makes the system easier to understand and manage. The presentation layer focuses on user interaction, the application/API layer handles processing, the data access layer controls structured data operations, and the data storage layer keeps the required information.

This pattern also supports modularity. Since the project contains several modules such as product catalog, cart, wishlist, checkout, order tracking, admin product management, category management, order management, customer message management, and content management, a layered structure helps keep these modules organized.

Maintainability is another important reason for choosing this pattern. If one part of the system needs to be improved in the future, it can be updated without changing the entire application. For example, product display can be improved in the presentation layer, while order processing can be improved in the API layer.

The pattern also supports scalability. As the business grows, new modules such as advanced reporting, delivery management, or extended promotional controls can be added more easily. In addition, the pattern supports easier testing because each part of the system can be checked based on its responsibility, such as interface testing, API testing, data validation, and storage verification.

4.2 Activity Diagram

Activity diagrams are used to show the step-by-step workflow of important system operations. In the Pure Haven BD system, activity diagrams are useful for understanding how Customer/Visitor and Admin users complete their tasks. These diagrams help explain the flow of actions, decisions, and system responses for major functional areas.

Figure 4.1 Activity Diagram for Product Browsing

This diagram will show how a Customer/Visitor enters the website, opens the shop or product section, browses available products, applies search or category filtering, views product results, and opens the product details page. The diagram should focus on the product discovery process without including any customer account or registration activity.

Figure 4.2 Activity Diagram for Cart and Checkout

This diagram will show how a Customer/Visitor selects a product, adds it to the cart, reviews cart items, updates quantity if required, proceeds to checkout, enters required customer and delivery information, selects a payment method from Cash on Delivery, bKash, or Nagad, and places the order. The flow should end with order success confirmation.

Figure 4.3 Activity Diagram for Order Tracking

This diagram will show how a Customer/Visitor opens the order tracking page, enters the required order-related information, submits the request, and views the current order status. The diagram should represent the interaction between the tracking interface and the order information stored in the system.

Figure 4.4 Activity Diagram for Admin Product Management

This diagram will show how the Admin opens the product management section, views the product list, chooses to add, edit, or delete a product, enters or updates product information, uploads a product image when required, saves the product, and receives confirmation from the system.

Figure 4.5 Activity Diagram for Admin Order Management

This diagram will show how the Admin opens the order management section, views the order list, searches or filters orders, opens order details, checks customer and product information, updates the order status, and saves the updated order information.

Figure 4.6 Activity Diagram for Customer Message Submission

This diagram will show how a Customer/Visitor opens the message or contact option, enters message information, submits the message, and the system stores the submitted message for Admin review. The diagram should also show that the Admin can later view and manage the submitted message from the admin panel.

4.3 Swim-lane Diagram

Swim-lane diagrams are used to show responsibilities across different users or system parts. For Pure Haven BD, swim-lane diagrams help clarify how Customer/Visitor, Admin, frontend interface, API layer, and storage layer work together during important system operations. These diagrams are useful because the project includes both public website workflows and admin-side management workflows.

Figure 4.7 Swim-lane Diagram for Customer Purchase Flow

This diagram will show the responsibilities of Customer/Visitor, public website interface, cart system, order API, and data storage during the purchase process. The flow should include product selection, cart review, checkout, payment method selection, order placement, and order confirmation.

Figure 4.8 Swim-lane Diagram for Admin Product Management

This diagram will show the responsibilities of Admin, admin panel interface, upload API, product API, and data storage during product management. The flow should include opening the product management section, entering product information, uploading an image when required, saving product information, and updating the product list.

Figure 4.9 Swim-lane Diagram for Order Tracking

This diagram will show the responsibilities of Customer/Visitor, tracking interface, order API, and data storage during the order tracking process. The flow should include entering order-related information, validating the tracking request, retrieving order status, and displaying the result to the Customer/Visitor.

Figure 4.10 Swim-lane Diagram for Customer Message Management

This diagram will show the responsibilities of Customer/Visitor, message form, message API, message storage, and Admin during message management. The flow should include message submission by the Customer/Visitor, message storage by the system, and message review or management by the Admin.

4.4 Class Diagram

The class diagram of Pure Haven BD represents the main entities used in the system and their relationships. Since the project is an e-commerce management system, the main classes are related to products, categories, orders, homepage content, customer messages, and site settings. The class diagram helps explain how the system organizes data and supports functional operations.

Product

The Product class represents the products available in the Pure Haven BD shop. It includes product-related information such as product name, price, image, category, description, stock-related data, and other display information. Products are shown to Customer/Visitor users and managed by the Admin.

ProductVariant

The ProductVariant class represents product variations such as size, label, price, stock, or variant-related details. A product may have one or more variants depending on the type of item being sold. This class supports flexible product presentation and management.

Order

The Order class represents customer order information. It contains customer details, delivery information, payment method selection, payment status, order status, and order-related summary information. Orders are created during checkout and managed by the Admin from the order management section.

OrderItem

The OrderItem class represents the individual products included in an order. Each order can contain multiple order items, and each order item is connected to a product. This class helps maintain product quantity, selected item details, and price-related information inside an order.

Category

The Category class represents the main product categories used to organize the product catalog. Categories help Customer/Visitor users browse products more easily and help the Admin maintain a structured product management process.

Subcategory

The Subcategory class represents smaller divisions under a category. It supports more specific product filtering and helps organize the product catalog in a more detailed way.

HomeSlide

The HomeSlide class represents homepage slider content. It is used to manage visual promotional content displayed on the homepage. Admin can manage slider-related content from the admin side.

CustomerMessage

The CustomerMessage class represents messages or contact requests submitted by Customer/Visitor users. These messages are stored for Admin review and management.

AdminAuth

The AdminAuth class represents admin authentication-related information used for admin panel access. It supports the separation between public customer-side features and admin-side management functions.

SiteSettings

The SiteSettings class represents site branding and general configuration information, such as site name and logo-related settings. These settings help maintain consistent identity across the website.

FooterSettings

The FooterSettings class represents footer-related information displayed on the public website. It supports the management of footer content such as contact-related text, links, or general site information.

Figure 4.11 Class Diagram of Pure Haven BD

The class diagram will be placed below this caption in the final report. The diagram should include the major classes Product, ProductVariant, Order, OrderItem, Category, Subcategory, HomeSlide, CustomerMessage, AdminAuth, SiteSettings, and FooterSettings. It should show the relationship between product and variants, category and subcategory, order and order items, and the supporting content and settings classes used by the system.
