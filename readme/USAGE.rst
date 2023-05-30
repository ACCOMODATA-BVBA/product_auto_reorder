Create new Rule Template

#. - Go to Inventory
#. - Select Menu Configuration -> Reordering Rule Templates
#. - Select Product Category and/or Product Attribute Values.
#. - Configure rule settings (min/max qty, warehouse, company etc.).
#. - Do not forget: Category and Product Attribute Values can be specified ONLY when Template is created!
#. - Reordeing rules will be created automatically for all products matching template

Create new Product

#. - Reordering rules will be created automatically when product is created if product category/attributes match any template
#. - Check "Don't create reordering rules from templates" if you do not want to create Reordering Rules automatically

Reordering Rules Templates are applied to ALL Products EXCEPT for the ones with "Don't create reordering rules from templates" enabled.
When new product is created the first matching Template is applied and reordering rules for the product are created.
First matching template is applied. Templates are searched in the following order:
1. Local Attributed: Product Attribute Values* AND Category are matching. `Click to get Pro Version! <https://apps.odoo.com/apps/modules/16.0/cx_product_auto_reorder_pro>`_
2. Local: Category is matching.
3. Global Attributed: Product Attribute Values* matching, Category not set.
4. Global: Product Attribute Values* and Category are not set.

When product category or attribute values are changed Reordering Rules Templates are applied again.
In case no new template can be applied old reordering rules for the product are deleted.

***Hint:*** to prevent automatic deletion or modification of reordering rules disable "Control via Template" in Reordering Rule form.

***Important notice:*** attribute values are joined using "AND" statement (e.g. "Size:L" AND "Color:White" AND "Model:Vintage").
It means that template will be applied to the product only if 'ALL' attribute values match.

**Warning! Product Category and Attribute Values cannot be changed once template is created!**
