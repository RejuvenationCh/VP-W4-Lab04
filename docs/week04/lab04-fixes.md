# Lab 04 Fix Log

- Problem : Category chips ran off the right edge on a small phone.
  Fix : Made the chip row scroll sideways so every category stays reachable.
  Checked : The small-phone test no longer reports a CategoryBar overflow, other widgets still overflow.

- Problem : The store name and rating overflowed to the right on a small phone.
  Fix : Let the header text use the available width, with wrapping or ellipsis for long lines.
  Checked : Small-phone portrait and landscape tests no longer report a StoreHeader overflow, other widgets still overflow.

- Problem : Two promo cards overflowed the right edge, and long names overflowed a card vertically.
  Fix : Made the promo strip scroll sideways and let card height follow its text, limiting long names to two lines.
  Checked : Small-phone portrait and landscape, plus the tablet long-name test, no longer report PromoStrip or PromoCard overflows
