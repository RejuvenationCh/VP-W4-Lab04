# Lab 04 Fix Log

- Problem : Category chips ran off the right edge on a small phone.
  Fix : Made the chip row scroll sideways so every category stays reachable.
  Checked : The small-phone test no longer reports a CategoryBar overflow, other widgets still overflow.

- Problem : The store name and rating overflowed to the right on a small phone.
  Fix : Let the header text use the available width, with wrapping or ellipsis for long lines.
  Checked : Small-phone portrait and landscape tests no longer report a StoreHeader overflow, other widgets still overflow.
