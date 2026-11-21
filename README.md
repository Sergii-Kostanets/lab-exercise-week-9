# Lab Exercise Week 9 - Bootstrap

**Name:** Sergii Kostanets

---

## Exercise 1 - Getting started with Bootstrap

### seaview.html

- **What the page looked like with and without the Bootstrap link:** Without the link the browser used its own default styles: a serif font (Times New Roman), an 8px margin around the body and plain headings. With the link Bootstrap's Reboot styles took over: a system sans-serif font, no body margin, adjusted heading sizes and line height. The page looked cleaner even before I added any classes.
- **What container did, and what container-fluid did at 1400 pixels:** At 1400 pixels `container` limited the content to 1320px wide and centred it, so there was empty space on both sides. Its width changes in steps at each breakpoint. `container-fluid` stretched the content across the full width of the window at every size. Both add 12px of padding on the left and right.
- **What display-4, text-center, lead and fw-bold changed:** `display-4` made the h1 much larger (3.5rem on a wide screen) and lighter (font weight 300). `text-center` centred the h1. `lead` made the header paragraph larger (1.25rem) and lighter, so it reads as an introduction. `fw-bold` made the h2 bold (font weight 700 instead of Bootstrap's default 500).
- **Margin and padding, in my own words:** Margin is space outside an element's border; it pushes other elements away and is always transparent. Padding is space inside the border, between the edge and the content, and it takes the element's background colour. In the class names `m` means margin, `p` means padding, `t` is top, `x` is left and right, and the number is the size: `3` is 1rem and `4` is 1.5rem. So `mt-3` adds 1rem above `main`, `p-4` adds 1.5rem inside it on every side, `px-4` adds 1.5rem inside the footer on the left and right only, and `m-0` removes the paragraph's default bottom margin.
- **Why container takes no dot:** The dot belongs to CSS, not HTML. In a style sheet `.container` is a selector that means "every element with the class container". In the `class` attribute I only write the name of the class, so it is `class="container"`.

### Puzzles: my predictions (before opening any page)

- **Puzzle 1:** Alpha largest, Gamma smallest, still h2
- **Puzzle 2:** Box B has centered text, container does not center text of Box A
- **Puzzle 3:** Box B margin top is 1 rem (16 px), Box C margin top is 3 rem (48 px), Box D is the tallest as it has margin top 1 rem and also paddings everywhere 1.5 rem. Box D larger then Box B by 3 rem (48 px).
- **Puzzle 4:** container and container-fluid have same width ar 400 px. At 800 px contaoner 720 px, container fluid 800 px. At 1400 container has 1320 px, container fluid 100% (1400px).
- **Puzzle 5:** At 400 px 1 image is 384 px, second is 480 px. Second does. At 100 first image still be 480 px. 
- **Puzzle 6:** First link looks like a button. Second looks like text because doesn't have a color and third looks like a link because does not have btn class.
- **For each wrong prediction: what the page showed, and why:**
- **Puzzle 5:** At 400 px 1st image is 376 px because .container has paddings everywhere 12 px, not 8 as I thought. 

### Tickets: what was wrong, and what I changed

- **Ticket 1:** remove dot at class=".container"
- **Ticket 2:** amend text-centre to text-center
- **Ticket 3:** replace mt3 with mt-3
- **Ticket 4:** take integriti token from console error and replace it in the link

### Validator results

Document checking completed. No errors or warnings to show.

---

## Exercise 2 - The Bootstrap grid

### grid-tiles.html

- **Why the third tile moved at step 3:** A row has 12 units. The columns asked for 4 + 4 + 6 = 14 units. After the first two tiles only 4 units were left, and the third tile needs 6, so it did not fit and moved down to the next line. There it takes half the width, on the left.
- **What col-auto did to the middle tile:** `col-auto` made the middle tile only as wide as its content (the word and its padding). The two `col` tiles shared the rest of the space equally, so they became wider and the middle one became narrow.
- **What offset-md-2 did, and why the notice is centred:** From 768 pixels up, `offset-md-2` adds 2 empty units before the column. The column takes 8 units, so 2 + 8 = 10 and 2 units stay free on the right. There are 2 units on each side, so the notice sits in the middle. Below 768 pixels neither class applies, and the notice is full width.
- **What justify-content-center and align-items-center did:** `justify-content-center` works along the line: the two `col-md-5` columns take 10 units, and it splits the 2 free units into one on each side, so the pair sits in the middle. `align-items-center` works up and down: normally the columns stretch to the same height, but with this class each keeps its own height and the short tile sits halfway down beside the tall one. At 400 pixels `col-md-5` does not apply, so the columns are full width and stack.

### shop-grid.html

- **Why six products belong in one row:** The `row` element is not one line on the screen; it is a container that wraps its columns onto as many lines as they need. With all six products in one row, the `row-cols` classes decide how many sit on each line at each width: one on a phone, two from 768 pixels, three from 992 pixels. If I wrote two rows of three, the lines would be fixed in groups of three. At 800 pixels that would give 2, 1, 2, 1, with a gap after each third product, instead of 2, 2, 2. The products also stay in one list, in the same order, at every width.
- **What row-cols-lg-3 counts:** It counts items across a line, not units out of twelve. From 992 pixels up it puts three columns on each line, so each one gets a third of the width. The class works out the width for me; I do not give each column `col-lg-4`.

### Puzzles: my predictions (before opening any page)

- **Puzzle 1:** 400 - 3, 800 - 3, 1200 - 3
- **Puzzle 2:** 400 - 2/1, 800 - 2/1, 1200 - 2/1, Three is alone
- **Puzzle 3:** 400 - 1, 800 - 3, 1200 - 3
- **Puzzle 4:** 400 - 1, 800 - 2, 1200 - 4
- **Puzzle 5:** 400 - 2 tiles on 4 lines, 800 - 4 tiles on 2 lines, 1200 - 4 tiles on 2 lines
- **Puzzle 6:** 400 - One takes the whole first line, Two takes the whole second line; 800 - One sits in the middle of the first line taking 6 grids, Two sits in the right of the second line taking 4 grids.
- **For each wrong prediction: what the page showed, and why:**

All correct

### Tickets: what was wrong, and what I changed

- **Ticket 1:** wrap column divs in a row div
- **Ticket 2:** fix col-md-5 to col-md-4
- **Ticket 3:** replace row-col-1 row-col-md-3 with row-cols-1 row-cols-md-3
- **Ticket 4:** change offset-md-2 to offset-md-1

### Validator results

Document checking completed. No errors or warnings to show.

---

## Exercise 3 - Components

### plant-home.html

- **How the navigation bar changes at 400 and 1200 pixels, and what the menu button does:** At 1200 the links show in the bar next to the brand. At 400 they are hidden and a menu button appears. Clicking it opens the links below the brand; clicking again closes them. Bootstrap's JavaScript does this.
- **What card, card-body and h-100 each do:** `card` makes the box with a border and rounded corners. `card-body` puts space around the text inside the card. `h-100` makes the card as tall as its column, so all cards in a row are the same height.
- **What happens when table is removed from the table's classes:** The Bootstrap table style goes away. The stripes, hover shade, borders and cell padding stop working, because those classes only work together with `table`.
- **What table-responsive does at 400 pixels:** It lets the table scroll sideways inside its own box. Only the table moves; the rest of the page stays still.
- **A, and button: when I would use each, in my own words:** I use `a` when clicking takes the visitor to another page or another place on the page. I use `button` when clicking does something on the page, like opening a menu or sending a form.

### Puzzles: my predictions (before opening any page)

- **Puzzle 1:**
- **Puzzle 2:**
- **Puzzle 3:**
- **Puzzle 4:**
- **Puzzle 5:**
- **Puzzle 6:**
- **For each wrong prediction: what the page showed, and why:**

### Tickets: what was wrong, and what I changed

- **Ticket 1:**
- **Ticket 2:**
- **Ticket 3:**
- **Ticket 4:**

### Validator results

---

## Exercise 4 - Forms, utilities and your own CSS

### enquiry.html

- **HTML, Bootstrap's feedback classes and JavaScript: what each one does for the validation:**
- **What the first button rule did, and the name of the rule that won:**
- **What the .brand-button rule does, and why a change in the Styles panel goes away on reload:**
- **Why a check in the browser is not enough:**

### Puzzles: my predictions (before opening any page)

- **Puzzle 1:**
- **Puzzle 2:**
- **Puzzle 3:**
- **Puzzle 4:**
- **Puzzle 5:**
- **Puzzle 6:**
- **For each wrong prediction: what the page showed, and why:**

### Tickets: what was wrong, and what I changed

- **Ticket 1:**
- **Ticket 2:**
- **Ticket 3:**
- **Ticket 4:**

### Validator results
