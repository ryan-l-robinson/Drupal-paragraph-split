# Drupal module: paragraphs split

When multiples of an item is adding to temporary fields and separated with ::, one paragraph for each is created instead.

## Scenario

This was initially developed to assist with importing data from an old Drupal 7 site into a new Drupal 9 site. One of the fields was a field collection reference on Drupal 7, allowing multiple collections associated with each node, where each collection has two fields. This could not be directly imported with feeds, so the solution included:

1. Exporting the data from the old site, where the multiples of each value is separated by ::
2. Importing with feeds, with feeds tamper splitting each into multiples of the temporary text fields.
3. This module then begins when the node is created, and translates the text fields into the paragraph, including associating those paragraphs with the node.

More on the context and how it was solved will be available soon at https://ryanrobinson.technology.

## Related

Another piece of this same task was handling the contact person for this node. A demo of this is available will be available in a different GitHub project.
