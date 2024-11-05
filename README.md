# Frequent Itemset Mining

This repository contains Java implementations of the **Apriori** and **FP-Growth** algorithms for discovering frequent itemsets in transactional databases.

## Usage

### Running the Apriori Implementation
1. **Compile**:
   ```bash
   javac Apriori.java
   ```
2. **Run**:
   ```bash
   java Apriori <input_file.csv> <support_value>
   ```
   **Example**:
   ```bash
   java Apriori groceries.csv 0.5
   ```

### Running the FP-Growth Implementation
1. **Compile** (assuming it's in `FPGrowth.java`):
   ```bash
   javac FPGrowth.java
   ```
2. **Run**:
   ```bash
   java FPGrowth <input_file.csv> <support_value>
   ```
   **Example**:
   ```bash
   java FPGrowth groceries.csv 0.5
   ```

## Input File Format
Each line of the CSV should represent a transaction with items separated by commas.

### Example `groceries.csv`
```plaintext
milk,bread,eggs
bread,butter
milk,bread,butter
eggs
```

## Output
Frequent itemsets will be printed along with their support values.
