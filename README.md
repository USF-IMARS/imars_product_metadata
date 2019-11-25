# imars_product_metadata
Information about IMaRS's satellite products and the imars_product_metadata SQL database.

Product metadata in the database starts at the `file` table.
The file` table holds metadata about each files catalogued by IMaRS.
Within this table the product_id and area_id columns are used to link to the `product` and `area` tables, respectively.
These tables contain detailed definitions of each area of interest and product type.

Within the `products` and `area` directories in this repo are markdown documents containing even more detailed information about the product types and areas of interest. 
