# Auction Lab

Live classroom auction simulations for economics and game theory courses. Runs entirely in the browser — no server, no dependencies to install.

## Folder Structure

```
/
├── index.html                    ← Landing page (start here)
├── auction-first-2-bidder.html   ← First-price sealed-bid simulation
├── slides/                       ← Upload lecture slides here (.pdf, .pptx)
│   └── .gitkeep
├── notes/                        ← Upload lecture notes here (.pdf, .docx)
│   └── .gitkeep
└── README.md
```

## How to Use

### Students
1. Open `index.html` (or the direct simulation link)
2. Enter Student ID → receive a random private value (0–100)
3. Submit a bid — repeat for all 10 rounds
4. After round 10, the student ID is locked out

### Instructor
1. Click the small dot in the **bottom-right corner** of the auction page
2. Enter the password: `first_84`
3. The instructor panel reveals:
   - All bids in a sortable table (filterable by round)
   - Scatter plot of Bid vs. Private Value with OLS trend line and optimal bid reference
   - Slope, intercept, and R² statistics
   - Excel download (one sheet per round + summary sheet)

## Adding Lecture Materials

1. Drop slide files (`.pdf` or `.pptx`) into the `slides/` folder
2. Drop note files (`.pdf` or `.docx`) into the `notes/` folder
3. Open `index.html` in a text editor and find the comments inside `#slidesList` and `#notesList`
4. Add links following the example format shown in the comments

```html
<!-- Example slide link -->
<a href="slides/lecture-01-intro.pdf" class="bucket-item" target="_blank">
  <span class="file-icon">📄</span> Lecture 01 — Introduction to Auctions
</a>
```

## Hosting on GitHub Pages

1. Push this folder to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder `/`
4. Your site will be live at `https://yourusername.github.io/your-repo-name/`

## Simulations

| Simulation | File | Status |
|---|---|---|
| First-Price Sealed Bid (2-Bidder) | `auction-first-2-bidder.html` | ✅ Live |
| Vickrey (Second-Price) | — | Coming soon |
| Common Value / Winner's Curse | — | Coming soon |
