# odoo-cheatsheet

### to-many write commands:

- `(0, _ , {'field': value})` creates a new record and links it to this one.
- `(1, id, {'field': value})` updates the values on an already linked record.
- `(2, id, _)` removes the link to and deletes the id-related record.
- `(3, id, _)` removes the link to, but does not delete, the id-related record. This is
usually what you will use to delete related records on many-to-many fields.
- `(4, id, _)` links an already existing record. This can only be used for many-to-
many fields.
- `(5, _, _)` removes all the links, without deleting the linked records.
- `(6, _, [ids])` replaces the list of linked records with the provided list.
