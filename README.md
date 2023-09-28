# Cooking-recipe-database


I am in the process of structuring a SQL database for a recipe website that I am playing around with.
Here is the table and the constraints .
 Recipe(table)
 - recipe_id (primary key)
 - recipe_name
 - recipe_description
 - course
 - food_category
 - cuisine
 - prep_time
 - cook_time

- Ingredients(table)
 - ingredient_id (primary key)
 - ingredient_name
 - recipe_id (foreign key)

- Quantity(table)
 - quantity_id (primary key)
 - recipe_id (foreign key)
 - ingredient_id (foreign key)
 - ingredient_quantity
 - ingredient_measurement

- Recipe Steps(table)
 - step_id (primary key)
 - step_description
 - recipe_id (foreign key)

- Join(table)*
 - join_id (primary key)
 - recipes_id(foreign key)
 - ingredients_id(foreign key)
 - quantity
