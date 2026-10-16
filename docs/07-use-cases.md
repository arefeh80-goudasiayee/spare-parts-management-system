# Use Case Documentation

## 1. Introduction

This document describes the main use cases of the Spare Parts Management System. It identifies the system actors and explains how they interact with the system to perform important tasks.

## 2. System Actors

| Actor ID | Actor Name | Description |
|---|---|---|
| A-01 | Customer | Searches for spare parts, views product details, places orders, and tracks orders. |
| A-02 | Store Manager | Manages products and updates order statuses. |

## 3. Use Case List

| Use Case ID | Use Case Name | Primary Actor | Description |
|---|---|---|---|
| UC-01 | Search Products | Customer | Allows customers to search for spare parts by name or product code. |
| UC-02 | View Product Details | Customer | Allows customers to view product prices, specifications, and availability. |
| UC-03 | Manage Shopping Cart | Customer | Allows customers to add products and change quantities in the cart. |
| UC-04 | Place Order | Customer | Allows customers to submit an order for selected products. |
| UC-05 | Track Order | Customer | Allows customers to check the current status of their orders. |
| UC-06 | View Own Orders | Customer | Allows customers to view their previously registered orders. |
| UC-07 | Add Product | Store Manager | Allows the manager to add a new spare part to the system. |
| UC-08 | Update Product | Store Manager | Allows the manager to modify product information. |
| UC-09 | Deactivate Product | Store Manager | Allows the manager to deactivate a product that is no longer available for sale. |
| UC-10 | Update Order Status | Store Manager | Allows the manager to update the status of a customer's order. |

## 4. Detailed Use Case: Place Order

**Use Case ID:** UC-04

**Use Case Name:** Place Order

**Primary Actor:** Customer

**Preconditions:**
- The customer can access the system.
- The required products are available in the product catalog.

**Main Flow:**
1. The customer searches for a spare part.
2. The system displays matching products.
3. The customer selects a product and views its details.
4. The customer adds the product to the shopping cart.
5. The customer reviews the cart and adjusts quantities if necessary.
6. The customer enters the required order information.
7. The system validates the order information.
8. The system checks product availability.
9. The system registers the order and generates a unique order ID.
10. The system displays an order confirmation and the order ID.

**Alternative Flows:**

- **Invalid Information:** If the order information is invalid, the system displays an error message and asks the customer to correct the information.
- **Insufficient Stock:** If the requested quantity is unavailable, the system informs the customer and asks them to update the cart.
- **Empty Cart:** If the shopping cart is empty, the system does not allow the customer to submit the order.

**Postconditions:**
- A valid order is stored in the system.
- A unique order ID is assigned to the order.
- The customer receives an order confirmation.

## 5. Use Case Diagram Description

The Use Case Diagram represents the interactions between the two main actors and the system.

- The Customer interacts with product search, product details, the shopping cart, order placement, and order tracking.
- The Store Manager interacts with product management and order status updates.
- The system boundary separates the system functions from external actors.

## 6. Activity Diagram Description

The Activity Diagram illustrates the workflow for placing an order.

The process starts when the customer searches for a product. The customer selects a product, adds it to the shopping cart, reviews the cart, and enters the required information. The system validates the information and checks product availability. If the information is invalid or stock is insufficient, the system displays an appropriate message. Otherwise, the order is registered, a unique order ID is generated, and a confirmation message is displayed.

## 7. Conclusion

These use cases describe the main interactions and order-processing workflow of the Spare Parts Management System. They provide a basis for requirements analysis, UML modeling, and future system development.
