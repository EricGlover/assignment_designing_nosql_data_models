
# Needs
* Products
  * Prices
  * Margin
* Departments
* Receipts
  * Profit
  * Sale-price (total)
  * Products
    * Quantity

  * Product

## Model

```javascript
  departmentsSWEETINDEX: {
    departmentsID: [productID, productID],
    departmentsID: [productID, productID],
    departmentsID: [productID, productID],
    departmentsID: [productID, productID],
    departmentsID: [productID, productID],
    departmentsID: [productID, productID]
  }
  departments: {
    departmentsID: {
      name: String,
      yourMom: true,
      products: [productID, productID]
    }
  }

  products: {
    productID: {
      price: Number,
      margin: Number,
      departmentID: Number
    }
  }

  Receipts: {
    ReceiptID: {
      profit: Number,
      totalSale: Number,
      date: String,
      user: userID,
      products: [
        {
          id: productID,
          salePrice: Number,
          profit: Number,
          quantity: Number
        }
      ]
    }
  }

```
