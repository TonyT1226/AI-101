# Deployment Guide

## Local Development

1. **Start the development server:**
   ```bash
   npm start
   # or
   python -m http.server 8000
   ```

2. **Access the application:**
   - Open your browser and navigate to `http://localhost:8000`
   - The application will automatically redirect to the home page

## Production Deployment

### Option 1: GitHub Pages
1. Push your code to a GitHub repository
2. Go to repository Settings > Pages
3. Select source branch (usually `main` or `master`)
4. Set root directory to `/public`
5. Your site will be available at `https://username.github.io/repository-name`

### Option 2: Netlify
1. Connect your GitHub repository to Netlify
2. Set build command: `echo "Static site - no build required"`
3. Set publish directory: `public`
4. Deploy automatically on push

### Option 3: Vercel
1. Connect your GitHub repository to Vercel
2. Set root directory to `public`
3. Deploy automatically on push

### Option 4: Traditional Web Server
1. Upload the contents of the `public/` directory to your web server
2. Ensure the server is configured to serve static files
3. Set up proper MIME types for HTML, CSS, and JavaScript files

## File Structure After Restructuring

```
AI 101/
├── public/                    # Static assets for production
│   ├── index.html            # Main entry point
│   ├── css/
│   │   └── style.css         # Main stylesheet
│   ├── js/
│   │   └── components.js     # JavaScript components
│   └── images/               # Image assets
│       ├── header.png
│       ├── sec3-reformat-table.png
│       ├── sidebar-hover.png
│       ├── sidebar-idle.png
│       └── template-pic.jpg
├── src/                      # Source code
│   ├── components/           # Reusable HTML components
│   │   ├── header.html
│   │   ├── navbar.html
│   │   └── footer.html
│   ├── pages/                # Page templates
│   │   ├── home.html
│   │   ├── training.html
│   │   └── resources.html
│   ├── utils/                # Utility functions (future)
│   └── styles/               # Component-specific styles (future)
├── package.json              # Project configuration
├── .gitignore               # Git ignore rules
├── README.md                # Project documentation
├── ai_training_prd.md       # Product requirements document
└── deploy.md                # This deployment guide
```

## Notes

- The `public/` directory contains all files needed for production deployment
- The `src/` directory contains source files that may need processing before deployment
- All file paths have been updated to reflect the new structure
- The application maintains the same functionality as before the restructuring 