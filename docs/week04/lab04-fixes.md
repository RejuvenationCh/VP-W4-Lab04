# Lab 04 Fix Log

Problem: Category chips ran off the right edge on a small phone.
Fix: Made the chip row scroll sideways so every category stays reachable.
Checked: The small phone test no longer reports a CategoryBar overflow.

Problem: The store name and rating overflowed to the right on a small phone.
Fix: Let the header text use the available width and shorten long lines with ellipsis.
Checked: Small phone portrait and landscape tests no longer report a StoreHeader overflow.

Problem: Two promo cards overflowed the right edge, and long names overflowed a card vertically.
Fix: Made the promo strip scroll sideways and let card height follow its text. Long names use at most two lines.
Checked: Small phone portrait and landscape tests and the tablet long name test no longer report promo card overflows.

Problem: Menu item names and prices overflowed the right edge on a small phone.
Fix: Put the name and price in the flexible part of each row. Long names use at most two lines.
Checked: Small phone portrait, landscape, and long name tests no longer report MenuTile overflows.

Problem: The cart summary and wide order button overflowed the right edge on a small phone.
Fix: Let the summary use the remaining width and let the button size to its label.
Checked: The 320 dp small phone portrait test passes.

Problem: The fixed sections of the screen were taller than the available space in landscape.
Fix: Put the header, search, categories, promos, and menu in one scrollable view. Menu items are built as needed.
Checked: All three landscape tests, both keyboard tests, and the 500 item test pass.

Problem: Tablet cards overflowed vertically because four square columns left too little room for their content.
Fix: Used two grid columns and limited long product names to two lines.
Checked: Tablet normal, long name, and dark mode tests pass.
