<!-- ╔══════════════════════════════════════════════════════════════════════════╗ -->
<!-- ║           SUPERMARKET BILLING SYSTEM - README                          ║ -->
<!-- ╚══════════════════════════════════════════════════════════════════════════╝ -->

<div align="center">

```
███████╗██╗   ██╗██████╗ ███████╗██████╗ ███╗   ███╗ █████╗ ██████╗ ██╗  ██╗███████╗████████╗
██╔════╝██║   ██║██╔══██╗██╔════╝██╔══██╗████╗ ████║██╔══██╗██╔══██╗██║ ██╔╝██╔════╝╚══██╔══╝
███████╗██║   ██║██████╔╝█████╗  ██████╔╝██╔████╔██║███████║██████╔╝█████╔╝ █████╗     ██║   
╚════██║██║   ██║██╔═══╝ ██╔══╝  ██╔══██╗██║╚██╔╝██║██╔══██║██╔══██╗██╔═██╗ ██╔══╝     ██║   
███████║╚██████╔╝██║     ███████╗██║  ██║██║ ╚═╝ ██║██║  ██║██║  ██║██║  ██╗███████╗   ██║   
╚══════╝ ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═╝╚═╝     ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝╚══════╝   ╚═╝  
                                                                                               
    ██████╗ ██╗██╗     ██╗     ██╗███╗   ██╗ ██████╗      ███████╗██╗   ██╗███████╗████████╗███████╗███╗   ███╗
    ██╔══██╗██║██║     ██║     ██║████╗  ██║██╔════╝      ██╔════╝╚██╗ ██╔╝██╔════╝╚══██╔══╝██╔════╝████╗ ████║
    ██████╔╝██║██║     ██║     ██║██╔██╗ ██║██║  ███╗     ███████╗ ╚████╔╝ ███████╗   ██║   █████╗  ██╔████╔██║
    ██╔══██╗██║██║     ██║     ██║██║╚██╗██║██║   ██║     ╚════██║  ╚██╔╝  ╚════██║   ██║   ██╔══╝  ██║╚██╔╝██║
    ██████╔╝██║███████╗███████╗██║██║ ╚████║╚██████╔╝     ███████║   ██║   ███████║   ██║   ███████╗██║ ╚═╝ ██║
    ╚═════╝ ╚═╝╚══════╝╚══════╝╚═╝╚═╝  ╚═══╝ ╚═════╝      ╚══════╝   ╚═╝   ╚══════╝   ╚═╝   ╚══════╝╚═╝     ╚═╝
```

### 🏪 A Console-Based Retail Management System Built in C

[![Language](https://img.shields.io/badge/Language-C-blue?style=for-the-badge&logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Standard](https://img.shields.io/badge/Standard-C99-blue?style=for-the-badge)](https://en.wikipedia.org/wiki/C99)
[![Platform](https://img.shields.io/badge/Platform-Linux%20%7C%20Windows%20%7C%20macOS-lightgrey?style=for-the-badge)](https://en.wikipedia.org/wiki/Cross-platform_software)
[![Build](https://img.shields.io/badge/Build-GCC%20%7C%20Make-orange?style=for-the-badge&logo=gnu&logoColor=white)](https://gcc.gnu.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen?style=for-the-badge)]()
[![Lines](https://img.shields.io/badge/Lines%20of%20Code-2000%2B-red?style=for-the-badge)]()
[![Modules](https://img.shields.io/badge/Modules-8-purple?style=for-the-badge)]()

---

> **A full-featured supermarket billing engine** — hash-table barcode lookups, dynamic cart management,  
> GST + bulk-discount math, binary file persistence, and a live admin dashboard. All in pure C. No GUI, no external libs.

---

</div>

## 📋 Table of Contents

| # | Section |
|---|---------|
| 1 | [Project Overview](#-project-overview) |
| 2 | [Key Features](#-key-features) |
| 3 | [System Architecture](#-system-architecture) |
| 4 | [Data Structures](#-data-structures) |
| 5 | [Hash Table — Barcode Engine](#-hash-table--barcode-engine) |
| 6 | [Module Breakdown](#-module-breakdown) |
| 7 | [Discount & Tax Algorithm](#-discount--tax-algorithm) |
| 8 | [File Handling](#-file-handling) |
| 9 | [Directory Structure](#-directory-structure) |
| 10 | [Build & Run](#-build--run) |
| 11 | [Menu Navigation](#-menu-navigation) |
| 12 | [Sample Output](#-sample-output) |
| 13 | [Test Cases](#-test-cases) |
| 14 | [Input Validation Rules](#-input-validation-rules) |
| 15 | [Concepts Demonstrated](#-concepts-demonstrated) |
| 16 | [Author](#-author) |

---

## 🎯 Project Overview

The **Supermarket Billing System with Barcode Simulation** is a console-based retail management application written in **pure C**. It simulates a real-world point-of-sale system by implementing fast barcode-to-product lookups via a **hash table**, a dynamic shopping cart, automatic GST + bulk-discount calculations, binary file persistence, and a full admin analytics dashboard — all without any external libraries or GUI frameworks.

This project is a practical demonstration of core **Data Structures & Algorithms**, **Systems Programming**, and **File I/O** in C — making it ideal for placement portfolios and academic project showcases.

---

## ✨ Key Features

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                         FEATURE HIGHLIGHTS                                  │
├──────────────────────────────────┬──────────────────────────────────────────┤
│  🔍  Hash Table Barcode Lookup   │  O(1) average product search by barcode  │
│  🛒  Dynamic Shopping Cart       │  Add, remove, update items in real-time  │
│  💰  Discount Engine             │  Bulk discounts: 5% / 10% / 15%          │
│  🧾  GST Calculation             │  Automatic 12% GST on discounted total   │
│  🖨️  Receipt Generation          │  Formatted professional bill receipts    │
│  📦  Inventory Management        │  Real-time stock tracking & deduction    │
│  ⚠️  Smart Alerts               │  Low stock + expiry date alerts          │
│  📁  Binary File Persistence     │  All data saved across sessions          │
│  📊  Admin Dashboard             │  Revenue, sales, top products analytics  │
│  ✅  Input Validation            │  Guards on every user input field        │
│  📝  Activity Logging            │  Text-based .log file for all actions    │
│  🏷️  Barcode Generator          │  Auto-generate barcodes from product ID  │
└──────────────────────────────────┴──────────────────────────────────────────┘
```

---

## 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────────────────────────────────┐
│                        SUPERMARKET BILLING SYSTEM                               │
│                              ARCHITECTURE                                       │
└─────────────────────────────────────────────────────────────────────────────────┘

                              ┌────────────────┐
                              │   main()       │
                              │  supermarket.c │
                              └───────┬────────┘
                                      │
              ┌───────────────────────┼──────────────────────┐
              │                       │                      │
     ┌────────▼───────┐    ┌──────────▼──────────┐   ┌──────▼──────────┐
     │ product_module │    │  barcode_module      │   │   cart_module   │
     │                │    │                      │   │                 │
     │ • addProduct   │    │ • generateBarcode    │   │ • addToCart     │
     │ • searchByName │    │ • simulateScan       │   │ • displayCart   │
     │ • updateProduct│    │ • enterManually      │   │ • removeItem    │
     │ • deleteProduct│    │ • addToBarcodeHash   │   │ • updateQty     │
     │ • categoryList │    │ • searchByBarcode    │   │ • clearCart     │
     └────────┬───────┘    └──────────┬───────────┘   └──────┬──────────┘
              │                       │                       │
              └───────────────────────▼───────────────────────┘
                                      │
              ┌───────────────────────┼──────────────────────┐
              │                       │                      │
     ┌────────▼────────┐   ┌──────────▼────────┐   ┌────────▼────────┐
     │ billing_module  │   │ inventory_module   │   │  admin_module   │
     │                 │   │                    │   │                 │
     │ • calcDiscount  │   │ • updateInventory  │   │ • dashboard     │
     │ • calculateGST  │   │ • lowStockAlert    │   │ • totalRevenue  │
     │ • calcTotalBill │   │ • expiryAlert      │   │ • categorySales │
     │ • processPayment│   │ • reorderSuggestion│   │ • topProducts   │
     └────────┬────────┘   └──────────┬─────────┘   └────────┬────────┘
              │                       │                       │
              └───────────────────────▼───────────────────────┘
                                      │
                          ┌───────────▼────────────┐
                          │    receipt_module       │
                          │                         │
                          │  • generateReceipt      │
                          │  • saveBillToHistory    │
                          │  • printFormattedBill   │
                          └───────────┬─────────────┘
                                      │
              ┌───────────────────────▼───────────────────────┐
              │                 FILE LAYER                     │
              │                                                │
              │  products.dat  │  bills.dat  │  inventory.dat  │
              │  barcode_hash.dat            │  supermarket.log│
              └────────────────────────────────────────────────┘
```

---

## 🗂️ Data Structures

### `Product` — Core Entity

```c
typedef struct Product {
    int   productID;           // Unique identifier
    char  barcode[15];         // Barcode string (e.g., "FOOD010015")
    char  productName[50];     // Display name
    char  category[30];        // Grocery / Frozen / Dairy / etc.
    char  brand[30];           // Brand name
    float price;               // Selling price (₹)
    float mrp;                 // Maximum retail price (₹)
    int   quantity;            // Current stock count
    int   minQuantity;         // Reorder trigger threshold
    int   maxQuantity;         // Max stock capacity
    char  supplier[50];        // Supplier name
    int   expiryDate;          // Expiry year (e.g., 2027)
    char  unit[10];            // "Kg" / "Liter" / "Piece"
    char  status[20];          // "Available" / "Discontinued"
} Product;
```

---

### `ProductDatabase` — With Embedded Hash Table

```c
typedef struct ProductDatabase {
    Product products[MAX_PRODUCTS];          // Product array (up to 1000)
    int     count;                           // Current product count
    int     barcodeHash[BARCODE_HASH_SIZE];  // Hash table: hashValue → index
} ProductDatabase;
```

---

### `CartItem` & `ShoppingCart`

```c
typedef struct CartItem {
    int   productID;
    char  productName[50];
    char  barcode[15];
    float price;
    int   quantity;
    float total;              // price × quantity
} CartItem;

typedef struct ShoppingCart {
    CartItem items[MAX_CART_ITEMS];  // Up to 100 items
    int      itemCount;
    float    totalAmount;            // Subtotal
    float    discountAmount;         // Bulk discount applied
    float    gstAmount;              // 12% GST
    float    finalAmount;            // After discount + GST
} ShoppingCart;
```

---

### `Bill` & `BillingHistory`

```c
typedef struct Bill {
    int   billID;
    char  customerName[50];
    char  phone[15];
    int   itemCount;
    float subtotal;
    float discount;
    float gst;
    float total;
    char  paymentMode[20];
    long  billDate;           // Unix timestamp
} Bill;

typedef struct BillingHistory {
    Bill bills[MAX_BILLS];    // Up to 500 bills
    int  count;
} BillingHistory;
```

---

## 🔑 Hash Table — Barcode Engine

The fastest operation in this system. Barcode → Product lookup runs in **O(1)** average time using a direct-address hash table of size 10,000.

```
HOW THE BARCODE HASH TABLE WORKS
═══════════════════════════════════════════════════════════════════

  Barcode String: "FOOD010015"
          │
          ▼
  hashValue = atoi("FOOD010015") % 10000
            = 10015 % 10000
            = 15
          │
          ▼
  barcodeHash[15]  →  productIndex = 0
          │
          ▼
  products[0]  →  { "Milk Fuller 1L", ₹80, qty:100 ... }


  HASH TABLE LAYOUT (barcodeHash[10000]):
  ┌───────┬──────────────────────────────────────────┐
  │ Index │ Value (product array index, or -1)       │
  ├───────┼──────────────────────────────────────────┤
  │   -1  │ (empty slot, default)                    │
  │   15  │  0  → products[0]  = Milk Fuller 1L      │
  │   26  │  1  → products[1]  = Aloo Paratha        │
  │   37  │  2  → products[2]  = Orange Juice        │
  │  ...  │  ...                                     │
  └───────┴──────────────────────────────────────────┘

  COLLISION HANDLING:
  If barcodeHash[hashVal] exists but barcode strings don't match
  → Falls back to linear scan through products[]
  → Rare case; average case remains O(1)
```

**Implementation:**

```c
// Initialize all slots to -1 (empty)
void initializeBarcodeHash(ProductDatabase* db) {
    for (int i = 0; i < BARCODE_HASH_SIZE; i++)
        db->barcodeHash[i] = -1;
}

// Insert: compute hash, store product index
void addToBarcodeHash(ProductDatabase* db, char barcode[], int productIndex) {
    int hashValue = atoi(barcode) % BARCODE_HASH_SIZE;
    db->barcodeHash[hashValue] = productIndex;
}

// Lookup: O(1) average, O(n) worst case (collision)
Product* searchByBarcode(ProductDatabase* db, char barcode[]) {
    int hashValue    = atoi(barcode) % BARCODE_HASH_SIZE;
    int productIndex = db->barcodeHash[hashValue];

    if (productIndex != -1 &&
        strcmp(db->products[productIndex].barcode, barcode) == 0)
        return &db->products[productIndex];

    // Fallback: linear scan on collision
    for (int i = 0; i < db->count; i++)
        if (strcmp(db->products[i].barcode, barcode) == 0)
            return &db->products[i];

    return NULL;  // Not found
}
```

---

## 📦 Module Breakdown

| File | Responsibility | Key Functions | ~Lines |
|------|---------------|---------------|--------|
| `supermarket.c` | Entry point, main menu, orchestration | `main()`, `displayMainMenu()`, all sub-menus | 750+ |
| `product_module.c` | CRUD on product database | `addProduct()`, `searchProduct()`, `updateProduct()`, `deleteProduct()`, `productReport()` | 180 |
| `barcode_module.c` | Barcode generation, scanning simulation, hash ops | `generateBarcode()`, `simulateBarcodeScan()`, `enterBarcodeManually()`, `addToBarcodeHash()` | 150 |
| `cart_module.c` | Shopping cart lifecycle | `addToCart()`, `displayCart()`, `removeItem()`, `updateQuantity()`, `clearCart()` | 160 |
| `billing_module.c` | Discount + GST math, bill summary | `calculateDiscount()`, `calculateGST()`, `calculateTotalBill()`, `processPayment()` | 180 |
| `inventory_module.c` | Stock deduction, alerts | `updateInventory()`, `lowStockAlert()`, `expiryAlert()` | 140 |
| `receipt_module.c` | Formatted receipt printing & bill history | `generateReceipt()`, `saveBill()`, `viewBills()`, `searchBill()` | 120 |
| `admin_module.c` | Analytics dashboard | `adminDashboard()`, `totalRevenue()`, `topSellingProducts()`, `categorySales()` | 120 |

---

## 💰 Discount & Tax Algorithm

```
BILLING CALCULATION FLOW
══════════════════════════════════════════════════════════════════

  Step 1: Sum up cart totals
  ───────────────────────────
  totalQuantity = Σ cart.items[i].quantity
  subtotal      = Σ cart.items[i].total


  Step 2: Apply Bulk Discount
  ────────────────────────────
  totalQuantity ≥ 50  →  discountRate = 15%
  totalQuantity ≥ 20  →  discountRate = 10%
  totalQuantity ≥ 10  →  discountRate =  5%
  totalQuantity  < 10 →  discountRate =  0%

  discountAmount   = subtotal × discountRate
  discountedAmount = subtotal − discountAmount


  Step 3: Apply GST (12%)
  ────────────────────────
  gstAmount   = discountedAmount × 0.12


  Step 4: Final Total
  ────────────────────
  finalAmount = discountedAmount + gstAmount


  EXAMPLE (8 items, ₹760 subtotal):
  ──────────────────────────────────
  Subtotal      :   ₹ 760.00
  Discount (0%) : − ₹   0.00
  After Discount:   ₹ 760.00
  GST (12%)     : + ₹  91.20
                  ──────────
  FINAL TOTAL   :   ₹ 851.20


  EXAMPLE (25 items, ₹1500 subtotal):
  ─────────────────────────────────────
  Subtotal      :   ₹1500.00
  Discount (10%): − ₹ 150.00
  After Discount:   ₹1350.00
  GST (12%)     : + ₹ 162.00
                  ──────────
  FINAL TOTAL   :   ₹1512.00
```

---

## 📁 File Handling

| File | Format | Mode Used | Contents |
|------|--------|-----------|----------|
| `products.dat` | Binary | `rb+` / `wb+` | Full `ProductDatabase` struct |
| `inventory.dat` | Binary | `rb+` / `wb+` | Stock quantities snapshot |
| `bills.dat` | Binary | `ab+` / `rb` | All `Bill` records |
| `barcode_hash.dat` | Binary | `rb+` / `wb+` | `barcodeHash[10000]` array |
| `supermarket.log` | Text | `a` | Timestamped activity log |

```c
// Save products database
void saveProducts(ProductDatabase* db) {
    FILE* fp = fopen(PRODUCTS_FILE, "wb");
    if (!fp) { perror("Cannot open products.dat"); return; }
    fwrite(db, sizeof(ProductDatabase), 1, fp);
    fclose(fp);
}

// Load products database
void loadProducts(ProductDatabase* db) {
    FILE* fp = fopen(PRODUCTS_FILE, "rb");
    if (!fp) { initializeBarcodeHash(db); db->count = 0; return; }
    fread(db, sizeof(ProductDatabase), 1, fp);
    fclose(fp);
}

// Append bill to history
void saveBill(Bill* bill) {
    FILE* fp = fopen(BILLS_FILE, "ab");
    if (!fp) { perror("Cannot open bills.dat"); return; }
    fwrite(bill, sizeof(Bill), 1, fp);
    fclose(fp);
}

// Log activity
void logActivity(char* action) {
    FILE* fp = fopen(SUPERMARKET_LOG, "a");
    if (!fp) return;
    time_t now = time(NULL);
    fprintf(fp, "[%s] %s\n", ctime(&now), action);
    fclose(fp);
}
```

---

## 🗃️ Directory Structure

```
supermarket-billing-system/
│
├── 📄  supermarket.c          ← Main file (750+ lines) — menu & orchestration
├── 📄  product_module.c       ← Product CRUD + category/report functions
├── 📄  barcode_module.c       ← Barcode generation, scan simulation, hash ops
├── 📄  cart_module.c          ← Cart lifecycle management
├── 📄  billing_module.c       ← Discount + GST math + bill summary
├── 📄  inventory_module.c     ← Stock deduction + alert system
├── 📄  receipt_module.c       ← Receipt formatting + bill history
├── 📄  admin_module.c         ← Analytics dashboard + revenue stats
│
├── 📂  data/                  ← Auto-created at runtime
│   ├── products.dat           ← Binary: product database
│   ├── inventory.dat          ← Binary: stock snapshots
│   ├── bills.dat              ← Binary: billing history
│   └── barcode_hash.dat       ← Binary: hash table dump
│
├── 📄  supermarket.log        ← Text: timestamped activity log
├── 📄  Makefile               ← Build automation
└── 📄  README.md              ← This file
```

---

## 🔧 Build & Run

### Prerequisites

```bash
# Linux / macOS
sudo apt install gcc make        # Debian/Ubuntu
brew install gcc                 # macOS

# Windows
# Install MinGW or use WSL
```

### Build with Makefile

```bash
# Clone repository
git clone https://github.com/snehalathaArakkonam/supermarket-billing-system.git
cd supermarket-billing-system

# Build all modules
make

# Run the system
./supermarket
```

### Build Manually

```bash
gcc -o supermarket \
    supermarket.c \
    product_module.c \
    barcode_module.c \
    cart_module.c \
    billing_module.c \
    inventory_module.c \
    receipt_module.c \
    admin_module.c \
    -lm -Wall -std=c99

./supermarket
```

### Makefile

```makefile
CC      = gcc
CFLAGS  = -Wall -std=c99 -lm
TARGET  = supermarket
SRCS    = supermarket.c product_module.c barcode_module.c cart_module.c \
          billing_module.c inventory_module.c receipt_module.c admin_module.c

all: $(TARGET)

$(TARGET): $(SRCS)
	$(CC) $(CFLAGS) -o $(TARGET) $(SRCS)

clean:
	rm -f $(TARGET) *.dat *.log

run: all
	./$(TARGET)
```

---

## 🗺️ Menu Navigation

```
MAIN MENU
═══════════════════════════════════════════
    SUPERMARKET BILLING SYSTEM
    Barcode Simulation
═══════════════════════════════════════════
1. Product Management
2. Barcode Scanner
3. Shopping Cart
4. Generate Bill
5. View Bills
6. Inventory Management
7. Admin Dashboard
8. Exit
═══════════════════════════════════════════
Enter choice: _


PRODUCT MANAGEMENT MENU          BARCODE SCANNER MENU
──────────────────────────        ──────────────────────────
1. Add Product                    1. Scan Barcode
2. Display All Products           2. Enter Barcode Manually
3. Search Product                 3. Add to Cart
4. Search by Barcode              4. Back to Main
5. Update Product
6. Delete Product                 SHOPPING CART MENU
7. Low Stock Products             ──────────────────────────
8. Product Report                 1. View Cart
9. Back to Main                   2. Clear Cart
                                  3. Update Quantity
BILLING MENU                      4. Remove Item
──────────────────────────        5. Back to Main
1. Calculate Total
2. Generate Receipt
3. Process Payment
4. Back to Main
```

---

## 🖥️ Sample Output

### Barcode Scan + Add to Cart

```
=== BARCODE SCANNER ===
Scan product barcode (or enter 0 to finish): FOOD010015

✅ Product Found!
 Barcode: FOOD010015
 Name: Milk Fuller 1L
 Price: ₹80.00
 Quantity: 100 Liter

Enter quantity to add: 5
✅ Added to cart: Milk Fuller 1L (Qty: 5 | Total: ₹400.00)
```

### Shopping Cart Display

```
========================================
    SHOPPING CART
========================================

1. Milk Fuller 1L
   Barcode: FOOD010015
   Price: ₹80.00 × 5 = ₹400.00

2. Aloo Paratha
   Barcode: FOOD010026
   Price: ₹120.00 × 3 = ₹360.00

========================================
Total Items: 2
Subtotal: ₹760.00
========================================
```

### Bill Summary

```
=== DISCOUNT CALCULATION ===
Total Items: 8
Discount Rate: 0% (No bulk discount)
Discount Amount: ₹0.00

=== GST CALCULATION ===
GST Rate: 12%
GST Amount: ₹91.20

========================================
    BILL SUMMARY
========================================
Total Items: 8
Subtotal: ₹760.00
Discount: ₹0.00
After Discount: ₹760.00
GST (12%): ₹91.20

FINAL TOTAL: ₹851.20
========================================
```

### Generated Receipt

```
========================================
       SUPERMARKET RECEIPT
========================================
Receipt ID: 1
Date: 25/06/2026
Cashier: Admin
----------------------------------------

Milk Fuller 1L
Barcode: FOOD010015
Qty: 5 × ₹80.00 = ₹400.00

Aloo Paratha
Barcode: FOOD010026
Qty: 3 × ₹120.00 = ₹360.00

========================================
Total Items: 2
Subtotal: ₹760.00
Discount: ₹0.00
GST (12%): ₹91.20
========================================
TOTAL AMOUNT: ₹851.20
========================================
Payment Mode: Cash
Thank you for shopping!
========================================
```

### Low Stock Alert

```
========================================
    LOW STOCK ALERTS
========================================

1. Orange Juice
   Barcode: FOOD010037
   Category: Beverages
   Available: 15
   Minimum: 20
   Status: ⚠️ LOW STOCK

Total Alerts: 1
========================================
```

### Admin Dashboard

```
========================================
    ADMIN DASHBOARD
========================================
Total Products   : 50
Total Sales Today: 120
Total Revenue    : ₹1,50,000.00
Low Stock Items  : 5
Expired Products : 0
----------------------------------------
TOP SELLING PRODUCTS:
1. Milk Fuller 1L     → 50 units
2. Aloo Paratha       → 35 units
3. Orange Juice       → 28 units
========================================
```

---

## 🧪 Test Cases

### TC-01: Add Product

```
Input:
  ID       : 1001
  Name     : Milk Fuller 1L
  Barcode  : FOOD010015
  Category : Grocery
  Brand    : Fresh Dairy
  Price    : 80
  MRP      : 100
  Qty      : 100
  Min Qty  : 20
  Max Qty  : 200
  Unit     : Liter
  Expiry   : 2027

Expected Output:
  ✅ Product added successfully!
  ✅ Barcode registered: FOOD010015
```

### TC-02: Search by Barcode (Hash Table)

```
Input  : FOOD010015
Process: hashValue = atoi("FOOD010015") % 10000 = 15
         barcodeHash[15] = 0
         products[0].barcode == "FOOD010015" ✓

Output :
  ✅ Found: Milk Fuller 1L
  Price   : ₹80.00
  Qty     : 100 Liter
  Category: Grocery
```

### TC-03: Bulk Discount (25 items)

```
Items   : 25 (≥ 20 → 10% discount)
Subtotal: ₹1500.00
Discount: ₹150.00 (10%)
After   : ₹1350.00
GST     : ₹162.00 (12%)
TOTAL   : ₹1512.00
```

### TC-04: Low Stock Trigger

```
Product   : Orange Juice
Qty       : 15
Min Qty   : 20
Condition : 15 < 20 → LOW STOCK
Output    : ⚠️ LOW STOCK ALERT! Please reorder.
```

### TC-05: Inventory Update After Sale

```
Product       : Milk Fuller 1L
Before Sale   : 100 units
Sold          : 5 units
After Sale    : 95 units
Saved to file : ✅ inventory.dat updated
```

---

## ✅ Input Validation Rules

| Field | Validation Rule |
|-------|----------------|
| Product ID | Must be unique, must be a positive integer |
| Barcode | Must be unique, alphanumeric, 10 chars |
| Product Name | Cannot be empty |
| Price | Must be a positive float |
| MRP | Must be ≥ Price |
| Quantity | Must be ≥ 0 |
| Min Quantity | Must be < Max Quantity |
| Expiry Date | Must be a future year |
| Customer Name | Cannot be empty |
| Phone Number | Must be exactly 10 digits |
| Cart Quantity | Cannot exceed available stock |

---

## 🎓 Concepts Demonstrated

```
COMPUTER SCIENCE CONCEPTS APPLIED
══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────┐
│  DATA STRUCTURES                                            │
│  ─────────────────────────────────────────────────────────  │
│  • Hash Table   → Barcode-to-Product mapping (O(1) lookup) │
│  • Struct Array → Product / Cart / Bill / History storage  │
│  • Linked Logic → Cart item chaining with index tracking   │
│                                                             │
│  ALGORITHMS                                                 │
│  ─────────────────────────────────────────────────────────  │
│  • Hashing      → atoi(barcode) % HASH_SIZE                │
│  • Linear Scan  → Fallback on hash collision               │
│  • Arithmetic   → Discount tiers + 12% GST formula        │
│  • Search       → Name/category substring matching        │
│                                                             │
│  FILE HANDLING                                              │
│  ─────────────────────────────────────────────────────────  │
│  • fwrite/fread → Binary struct serialization              │
│  • fprintf      → Text activity logging                    │
│  • fopen modes  → rb+, wb+, ab+ for different operations  │
│  • Error Check  → NULL file pointer handling              │
│                                                             │
│  SYSTEMS PROGRAMMING                                        │
│  ─────────────────────────────────────────────────────────  │
│  • Pointers     → Pass structs by reference for mutation  │
│  • Memory       → Stack-allocated arrays, pointer returns  │
│  • Modular C    → Multi-file compilation with shared types │
│  • String Ops   → strcmp, strcpy, sprintf, scanf guards   │
│                                                             │
│  SOFTWARE ENGINEERING                                       │
│  ─────────────────────────────────────────────────────────  │
│  • Separation of Concerns → 8 focused modules             │
│  • Input Validation       → All fields validated          │
│  • Error Handling         → File errors + invalid input   │
│  • Logging                → Timestamped activity trail    │
└─────────────────────────────────────────────────────────────┘
```

---

## 👩‍💻 Author

<div align="center">

**Snehalatha**
Final Year B.Tech — Computer Science & Engineering (AI/ML Specialization)

[![GitHub](https://img.shields.io/badge/GitHub-snehalathaArakkonam-black?style=for-the-badge&logo=github)](https://github.com/snehalathaArakkonam)
[![C Projects](https://img.shields.io/badge/Portfolio-C%20Projects-blue?style=for-the-badge&logo=c)](https://github.com/snehalathaArakkonam)

---

*Built as part of a C programming portfolio for placement preparation.*  
*Demonstrates mastery of DSA, file I/O, and modular systems programming in C.*

</div>

---

<div align="center">

```
╔══════════════════════════════════════════════════════════╗
║   Thank you for visiting this project!                  ║
║   Star ⭐ if you found it useful.                       ║
╚══════════════════════════════════════════════════════════╝
```

[![Made with C](https://img.shields.io/badge/Made%20with-C-blue?style=flat-square&logo=c)](https://en.wikipedia.org/wiki/C_(programming_language))
[![Portfolio](https://img.shields.io/badge/Part%20of-Portfolio%20Projects-orange?style=flat-square)](https://github.com/snehalathaArakkonam)

</div>
