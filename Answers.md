answer 1. Relationship Between “Product” and “Product_Category” Entities:
The relationship between the “Product” and “Product_Category” entities is established through the “category_id” attribute.
Specifically:
In the “Product” table, each product record includes a “category_id” that corresponds to a specific category.
In the “Product_Category” table, the “id” field uniquely identifies each category.
This relationship allows us to associate products with their respective categories. For example, a product with a certain “category_id” belongs to the corresponding category defined in the “Product_Category” table.

answer 2. Ensuring Valid Categories for Products: To ensure that each product in the “Product” table has a valid category assigned to it, consider the following approaches:
Foreign Key Constraints:
Implement foreign key constraints between the “category_id” in the “Product” table and the “id” in the “Product_Category” table.
This ensures that every category ID referenced in the “Product” table corresponds to a valid ID present in the “Product_Category” table.
Non-Nullable Category ID:
Make sure that the “category_id” field in the “Product” table is not nullable.
This means that every product must have a category ID assigned, preventing any orphaned or invalid records.

