# Development Guide

Made by Med Yessine Khmiri (student)

## Development Status

This project is actively under development. The development guide will be updated as new features are added and existing ones are improved. Your contributions and feedback are welcome!

## What is This Project?

This is a website that helps Tunisian people find and avoid brands that support occupation. The website is:

- Free and open source
- Made by the community
- Easy to use
- Available in English

## Project Structure

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

## Getting Started

### 1. Install Required Software

You need these tools to work on the project:

- Node.js (version 14 or newer)
  - Download from: https://nodejs.org/
  - This includes npm (Node Package Manager)
- Git (for version control)
  - Download from: https://git-scm.com/
- A code editor (like VS Code)
  - Download from: https://code.visualstudio.com/

### 2. Get the Code

1. Open your terminal
2. Run these commands:
   ```bash
   git clone https://github.com/Mohamed-Yessine-Khmiri/Boycott-TN.git
   cd BoyCott-Tunise
   ```

### 3. Install Dependencies

1. In the project folder, run:
   ```bash
   npm install
   ```
2. Wait for all packages to install

### 4. Start the Website

1. Run this command:
   ```bash
   node server.js
   ```
2. Open your browser
3. Go to: http://localhost:3000

## How to Add New Brands

### 1. Check Brand Information

All brands must be checked using [The Witness Boycott Database](https://boycott.thewitness.news/):

- Look for the brand on The Witness website
- Use this link format: https://boycott.thewitness.news/target/[brandname]
- Example: https://boycott.thewitness.news/target/cocacola

### 2. Add Brand Image

1. Find the brand's logo
2. Save it as PNG format
3. Put it in: `assets/images/products/`
4. Name it like: `brand-name.png`

### 3. Add Brand Data

1. Open `data/data.js`
2. Add new brand in this format:
   ```javascript
   {
     name: "Brand Name",
     image: "assets/images/products/brand-name.png",
     category: "Category Name",
     description: "Short description",
     proof: "Why we boycott this brand"
   }
   ```

### 4. Brand Categories

Use these categories:

- Bodycare
- Cleaning
- Cosmetics
- Drinks
- Entertainment
- Fashion
- Finance
- Food
- Haircare
- Snacks
- Supermarket
- Technology
- Travel
- Pharmaceuticals
- Famous People
- Others

## How to Help

### 1. Find Bugs

- Test the website
- Report problems
- Suggest fixes

### 2. Add Features

- New brand categories
- Better search
- More languages
- Better design

### 3. Improve Code

- Fix errors
- Make code faster
- Add tests
- Better security

## Best Practices

### 1. Code Style

- Use clear names
- Add comments
- Follow standards
- Keep it simple

### 2. Security

- Check user input
- Use safe passwords
- Keep data safe
- Update regularly

### 3. Testing

- Test all changes
- Check on phones
- Test in browsers
- Test security

## How to Deploy

### 1. Prepare

- Test everything
- Check security
- Update files
- Backup data

### 2. Deploy

- Choose hosting
- Set up server
- Upload files
- Start server

### 3. Monitor

- Check logs
- Watch errors
- Test speed
- Check security

## Need Help?

- Check [HELP.md](HELP.md) for technical details
- Open GitHub issue
- Contact admin
- Join community

## License

This project is MIT licensed. See [LICENSE](LICENSE) for details.

## Server Setup

### 1. Express Server (server.js)

The website uses Express.js for the backend:

- Handles API requests
- Serves static files
- Manages feedback
- Controls admin access

### 2. API Endpoints

The server provides these endpoints:

- GET /api/brands - Get all brands
- POST /api/feedback - Submit feedback
- GET /api/feedback - Get feedback (admin only)
- DELETE /api/feedback/:id - Delete feedback (admin only)

### 3. Security Features

- CORS enabled
- JSON parsing
- Error handling
- Admin authentication

## Feedback System

### 1. How It Works

- Users submit feedback through the website
- Feedback is stored in JSON files
- Admin can view and manage feedback
- Feedback includes:
  - User message
  - Timestamp
  - Contact info (optional)

### 2. Feedback Management

- View all feedback in admin panel
- Delete unwanted feedback
- Export feedback data
- Filter feedback by date

## Admin Panel

### 1. Access

- Located at /admin.html
- Password protected
- Secure login system
- Session management

### 2. Features

- View all feedback
- Delete feedback
- Monitor website usage
- Manage brand data
- Update website content
