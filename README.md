# imars_product_metadata
Information about IMaRS's satellite products and the imars_product_metadata SQL database.

Product metadata in the database starts at the `file` table.
The `file` table holds metadata about each files catalogued by IMaRS.
Within this table the product_id and area_id columns are used to link to the `product` and `area` tables, respectively.
These tables contain detailed definitions of each area of interest and product type.

Within the `products` and `area` directories in this repo are markdown documents containing even more detailed information about the product types and areas of interest. 
The `.md` markdown files are named to match `*.short_name` in the schema.

## Database Schema
The current database schema is defined by files over in [imars_puppet.../modules/role/files/sql](https://github.com/USF-IMARS/imars_puppet/tree/8e9d0c34bb74dd8378421e879020ef01deb300a4/modules/role/files/sql).
These files should be moved to a `./schema/` directory here and added to the `imars_puppet` repo as a submodule.
