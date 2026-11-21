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

## Exercise 2 - The Bootstrap grid

### grid-tiles.html

- **Why the third tile moved at step 3:**
- **What col-auto did to the middle tile:**
- **What offset-md-2 did, and why the notice is centred:**
- **What justify-content-center and align-items-center did:**

### shop-grid.html

- **Why six products belong in one row:**
- **What row-cols-lg-3 counts:**

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

## Exercise 3 - Components

### plant-home.html

- **How the navigation bar changes at 400 and 1200 pixels, and what the menu button does:**
- **What card, card-body and h-100 each do:**
- **What happens when table is removed from the table's classes:**
- **What table-responsive does at 400 pixels:**
- **A, and button: when I would use each, in my own words:**

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
