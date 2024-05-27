## E-commerce Sales Analysis with ETL and Data Mining

This project analyzes an e-commerce dataset to uncover valuable customer insights and sales trends. It utilizes ETL (Extract, Transform, Load) processes and data mining techniques to provide a comprehensive view of sales performance.

### Data Exploration

The dataset includes information on each transaction, such as product details, customer information, and transaction amounts. Key fields include:

* **InvoiceNo**: Unique identifier for each transaction
* **StockCode**: Product code
* **Description**: Product description
* **Quantity**: Number of products purchased per transaction
* **InvoiceDate**: Date and time of the transaction
* **UnitPrice**: Price per unit of the product
* **CustomerID**: Unique identifier for each customer
* **Country**: Customer's country of residence

### Data Preparation

The data undergoes cleaning and transformation steps to ensure accuracy and facilitate analysis:

* **Data Cleaning:** 
    * Rows with missing `CustomerID` or `Description` are removed.
    * Data types are corrected (e.g., `InvoiceDate` to datetime, `CustomerID` to integer).
* **Feature Engineering:**
    * A new column `TotalPrice` is created by multiplying `Quantity` and `UnitPrice`.

### Data Analysis

The cleaned data is loaded into an SQLite database for efficient querying and analysis. Data mining techniques are applied to extract valuable insights:

* **Sales Summary:** Provides a comprehensive overview of total sales.
* **Monthly Sales Trend:** Visualizes sales trends over time.
* **Top Customers:** Identifies customers with the highest purchase amounts.

### Technical Specifications

* Python 3.x
* Libraries: Pandas, NumPy, Matplotlib, SQLAlchemy

### Running the Analysis

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   ```

2. **Install required packages:**

   ```bash
   pip install pandas numpy matplotlib sqlalchemy
   ```

3. **Run the analysis script:**

   ```bash
   python analysis.py
   ```

### Contributing

We welcome contributions! Please fork the repository and submit a pull request with your changes.

### License

This project is licensed under the MIT License. Refer to the `LICENSE` file for details.