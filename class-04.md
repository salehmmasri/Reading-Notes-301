# Responsive Web Design and Regular Expressions

---

## A Complete Guide to Grid
*CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a dimensional system.*

## Properties for the Parent (Grid Container)

- display
    - Values: grid - generates a block-level grid inline-grid - generates an inline-level grid
- grid-template-columns/ grid-template-rows
    - Values: - can be a length, a percentage, or a fraction of the free space in the grid (using the fr unit) - an arbitrary name of your choosing
- grid-template-areas
    - Values: - the name of a grid area specified with grid-area . - a period signifies an empty grid cell none - no grid areas are defined
- grid-template - Values: none - sets all three properties to their initial values / - sets grid-template-columns and grid-template-rows to the specified values, respectively, and sets grid-template-areas to none etc...
- Properties for the Children (Grid Items)

- grid-column-start/ grid-column-end/ grid-row-start/ grid-row-end
    - Values: - can be a number to refer to a numbered grid line, or a name to refer to a named grid line span - the item will span across the provided number of grid tracks span - the item will span across until it hits the next line with the provided name auto - indicates auto-placement, an automatic span, or a default span of one
- grid-column/ grid-row - Values: / - each one accepts all the same values as the longhand version, including span etc..
*grid-column-start property. grid-column-end property. If you want to count grid lines from the right instead of the left, you can give grid-column-start and grid-column-end negative values. For example, you can set it to -1 to specify the first grid line from the right.*

`#garden { display: grid; grid-template-columns: 20% 20% 20% 20% 20%; grid-template-rows: 20% 20% 20% 20% 20%; }`

- #water `{ grid-column-start: 1; grid-column-end:-2; }`

- span keyword, span only works with positive values. #water { grid-column-start: 2; grid-column-end:span 2; }

- Typing both grid-column-start and grid-column-end every time can get tiring. Fortunately, grid-column is a shorthand property that can accept both values at once, separated by a slash. grid-column: 2 / 4; will set the grid item to start on the 2nd vertical grid line and end on the 4th grid line.

- One of the things that sets CSS grids apart from flexbox is that you can easily position items in two dimensions: columns and rows. grid-row-start works much like grid-column-start except along the vertical axis. grid-row #water { grid-row:3/6; }

- If typing out both grid-column and grid-row is too much for you, there's yet another shorthand for that. grid-area accepts four values separated by slashes: grid-row-start, grid-column-start, grid-row-end, followed by grid-column-end.

- One example of this would be grid-area: 1 / 1 / 3 / 6;.

- If grid items aren't explicitly placed with grid-area, grid-column, grid-row, etc., they are automatically placed according to their order in the source code. We can override this using the order property, which is one of the advantages of grid over table-based layout.

- By default, all grid items have an order of 0, but this can be set to any positive or negative value, similar to z-index.

- grid-template-columns For example, we previously defined five 20% columns with the rule grid-template-columns: 20% 20% 20% 20% 20%;. This can be simplified as grid-template-columns: repeat(5, 20%); #garden { display: grid; grid-template-columns:100px 3em 40%; grid-template-rows: 20% 20% 20% 20% 20%; }

- fr Grid also introduces a new unit, the fractional fr. Each fr unit allocates one share of the available space. For example, if two elements are set to 1fr and 3fr respectively, the space is divided into 4 equal shares; the first element occupies 1/4 and the second element 3/4 of any leftover space.

`#garden { display: grid; grid-template-columns:0.6fr 3fr; grid-template-rows: 20% 20% 20% 20% 20%;`
