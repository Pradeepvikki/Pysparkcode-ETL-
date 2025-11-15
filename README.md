# Pysparkcode-ETL-
✅ PySpark Notebook – End-to-End Workflow (GitHub Points)
1️⃣ Start Spark Session

Initialized a SparkSession in the PySpark notebook.

Configured required settings for local execution.

2️⃣ Load Dataset

Loaded the dataset using:

spark.read.csv()

Options like header=True, inferSchema=True

Verified successful loading with printSchema() and .show().

3️⃣ Data Display & Exploration

Displayed records using:

.show()

.limit()

.take()

.head()

Explored schema, data types, and record count:

.printSchema()

.columns

.count()

4️⃣ Basic DataFrame Operations

Selected specific columns using .select().

Renamed columns using .withColumnRenamed().

Dropped unwanted columns using .drop().

Removed duplicate rows using .dropDuplicates().

5️⃣ Data Cleaning & Transformation

Standardized column values using:

.withColumn()

trim(), lower(), upper()

regexp_replace()

Cleaned incorrect values such as:

Wrong date formats

Misspelled statuses

Invalid emails

Numeric columns in string/word format

6️⃣ Handling Missing Values

Used:

dropna() to remove NULL rows

fillna() to fill missing values

Converted invalid entries (e.g., NaN, words, symbols) to NULL.

7️⃣ Type Casting

Casted columns to correct data types:

cast(IntegerType())

cast(FloatType())

to_date() for date columns

Ensured numeric columns contain only numeric values.

8️⃣ Column Standardization

Standardized formats:

Customer IDs → C001, C002, etc.

Delivery Status → Delivered, Pending, etc.

Payment Mode → Credit Card, Debit Card, UPI

Rounded amounts to 2 decimals.

9️⃣ Full Dataset Cleanup

Applied a full cleaning pipeline:

Date normalization

Email validation

Removing special characters

Converting word-numbers to digits

Ensuring city names are valid

🔟 Final Output

Displayed cleaned DataFrame using .show().

Saved cleaned data as:

CSV

Parquet

JSON
