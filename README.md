# BoyCott Tunise

A free and open-source website that helps Tunisian people find and avoid brands that support occupation. Made with modern web tools.

Made by Med Yessine Khmiri (student)

## Open Source Commitment

This project is:

- 100% Free to use
- Open source under MIT License
- Made by the community
- Always free
- No hidden costs

## Where to Find the Code

https://github.com/Mohamed-Yessine-Khmiri/Boycott-TN.git

## Current Status

Website is Under Development

- Basic features are working at http://localhost:3000
- Made in Tunisia, for Tunisian people
- Made by the community
- In English
- Open source and free
- Still adding new features
- Looking for contributors

Note: This website is still being built. Some features may not work yet, and new features are being added regularly.

## Important Notice

All brand names, logos, and trademarks on this website belong to their owners. We only use them to show information. We do not own any of these brands.

This website helps people make better choices. All brand information is checked using [The Witness Boycott Database](https://boycott.thewitness.news/).

## Free to Use

This project is completely free:

- No payment required
- No subscription needed
- No hidden fees
- Free to modify
- Free to distribute

## How to Help

You can help by:

- Making the website look better
- Writing code
- Finding brands in Tunisia
- Writing better instructions
- Fixing problems
- Adding new features

Your help will make our boycott project stronger! See our [Development Guide](DEVELOPMENT.md) to start.

## What the Website Can Do

- List of brands to avoid
- Brands sorted by type
- Search for brands
- Send feedback
- Admin page for feedback
- Works on phones and computers
- Dark and light mode

## What You Need to Run the Website

- Node.js (version 14 or newer)
- npm (comes with Node.js)

## How to Start the Website

### Step 1: Open Terminal

Choose any of these:

- Press `Windows + R`, type `cmd` and press Enter
- Press `Windows + X` and choose "Windows PowerShell" or "Terminal"
- Open VS Code and press `` Ctrl + ` ``

### Step 2: Go to Project Folder

```
cd BoyCott-Tunise
```

Tip: You can right-click the project folder and choose "Open in Terminal"

### Step 3: Install Required Files

```
npm install
```

### Step 4: Start Website

```
node server.js
```

Success! When you see:

```
Server is running on http://localhost:3000
```

The website is ready!

### How to Use the Website

- Open your browser
- Go to: http://localhost:3000

### How to Stop the Website

Press `Ctrl + C` in the terminal

## How to Use the Admin Page

The admin page is at `http://localhost:3000/admin.html`. Here you can:

- See all feedback
- Delete feedback
- Watch how people use the website

Note: The admin page needs a password. Contact the admin to get access.

## How to Help

Want to help? See our [Development Guide](DEVELOPMENT.md) for:

- How to add new brands
- How to help
- How to set up your computer
- Best ways to code

## Website Structure

```
boycott-tn/
├── assets/              # Static assets
│   ├── images/         # Brand images and icons
│   ├── js/            # JavaScript files
│   └── styles/        # CSS styles
├── data/               # Data files
│   ├── feedback/      # User feedback storage
│   └── data.js        # Brand data
├── node_modules/       # Dependencies
├── .git/              # Git repository
├── admin.html         # Admin dashboard
├── index.html         # Main website
├── server.js          # Express server
├── feedbackManager.js # Feedback handling
├── package.json       # Project configuration
├── package-lock.json  # Dependency lock file
├── manifest.json      # Web app manifest
├── .gitignore        # Git ignore rules
├── README.md         # Project documentation
├── DEVELOPMENT.md    # Development guide
├── HELP.md           # Technical guide
└── LICENSE           # MIT License
```
