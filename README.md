<img width="1512" height="832" alt="image" src="https://github.com/user-attachments/assets/96d160c4-b74b-4654-add7-38ad7438c0be" />
# Mini_Project_1
Analysis_on_Credit_card_customers

-10,127 rows x 23 columns in the original dataset
-There are No blanks/null values, no duplicate rows, there are 3 columns with "Unknown" values

#Step 1- DATA CLEANING
1. Deleted two columns: Naive Bayes columns (model output from the dataset author, not customer data).
2. Standardised Status column: Existing Customer to Active, Attrited Customer to Churned.
3. Standardised Gender column: M to Male, F to Female
4. Renamed Unknown to Not Disclosed in Education, Marital Status and Income. (The rows were not deleted, since ~30% of customers have at least one Unknown)
5. Replaced income labels: Less than $40K to <$40K, $40K - $60K to $40K-$60K, $60K - $80K to $60K-$80K, $80K - $120K to $80K-$120K, $120K + to $120K+.
6. Renamed all 21 columns headers to simpler names
7. Changed Data types: Client ID as whole number (no scientific notation), Utilisation as percentage.
8. Added 7 new columns:
i. Added Churn Flag (1 if Churned) (for example: =IF(B2="Churned",1,0))
ii. Added Age Band.
iii.Added Tenure Band.
iv.Added Utilisation Band.
v.Added Credit Limit Band.
vi.Added Inactivity Band.
vii.Added Spend per Transaction (Trans Amount / Trans Count)


