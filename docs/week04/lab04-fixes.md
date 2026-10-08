# Lab 04 Fix Log

- Widget : CategoryBar
  Error / symptom : Chips ran past the right edge on a small phone.
  Rule broken : The Row's children needed more width than its parent provided.
  Fix : Made the chip row scroll horizontally.

- Widget : StoreHeader
  Error / symptom : Store name and rating overflowed to the right.
  Rule broken : The Row did not limit the width of its text.
  Fix : Gave the text flexible space and limited long lines.

- Widget : PromoStrip
  Error / symptom : Two cards did not fit across a small phone.
  Rule broken : The cards together were wider than the width passed down.
  Fix : Made the promo strip scroll horizontally.

- Widget : PromoCard
  Error / symptom : A long product name overflowed the card vertically.
  Rule broken : The fixed card height was smaller than its content.
  Fix : Let the card height follow its content and limited names to two lines.

- Widget : MenuTile
  Error / symptom : Item names and prices overflowed to the right.
  Rule broken : The Row gave its text more width than was available.
  Fix : Put the name and price in flexible space and limited long names.

- Widget : CartBar
  Error / symptom : Summary and order button overflowed to the right.
  Rule broken : Their combined widths exceeded the width from the parent.
  Fix : Let the summary use remaining space and the button size to its label.

- Widget : MenuScreen
  Error / symptom : Fixed sections overflowed the bottom in landscape.
  Rule broken : The Column's children were taller than the available height.
  Fix : Made the page one scrollable view with lazy menu items and a LayoutBuilder breakpoint.

- Widget : MenuCard
  Error / symptom : Tablet grid cards overflowed vertically.
  Rule broken : Four square grid cells left too little height for the card content.
  Fix : Used two grid columns and limited long names to two lines.

- Widget : MenuScreen
  Error / symptom : Zero items caused a crash.
  Rule broken : No constraint rule was broken. Reading missing promo items prevented layout.
  Fix : Added an empty state with an icon, message, and action, and handled fewer than two promos.

- Widget : CartBar
  Error / symptom : Order button sat under the gesture bar.
  Rule broken : The button was positioned inside the bottom system inset.
  Fix : Wrapped the cart bar in SafeArea.
