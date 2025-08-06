# Template Customization Guide

This guide will help you customize the terminal portfolio template for your own use.

## Quick Setup

1. **Fork or clone** this repository
2. **Replace all placeholder text** with your information
3. **Deploy** to your preferred hosting service

## Required Customizations

### 1. Personal Information

Replace these placeholders in `index.html`:

| Placeholder | What to Replace With |
|-------------|---------------------|
| `Your Name Here` | Your full name |
| `Your GitHub Username` | Your GitHub username |
| `Your LinkedIn Username` | Your LinkedIn username |
| `Your Website URL` | Your website URL (if you have one) |

### 2. Projects Section

Update the `PROJECTS` array in the JavaScript section:

```javascript
const PROJECTS = [
    {
        name: 'your-actual-project-name',
        owner: 'Your GitHub Username',
        fallbackDesc: 'Description of your project'
    },
    // Add more projects as needed
];
```

**Important**: The `name` should match your actual GitHub repository name, and the `owner` should be your GitHub username.

### 3. About Section

Customize the "About" section content to reflect your background and interests.

### 4. Contact Links

Update the contact section with your actual social media profiles.

## Optional Customizations

### Styling

The CSS is embedded in the HTML file. You can modify:
- Colors (currently green-on-black theme)
- Fonts (currently Consolas/Monaco)
- Layout and spacing
- Terminal appearance

### Performance Badge

The performance badge in the bottom-right corner shows "13KB | 100/100 | Vanilla". You can:
- Remove it entirely
- Update the size if your file changes
- Customize the styling

### Meta Tags

Update the meta description and other SEO-related tags to match your content.

## Deployment Options

### GitHub Pages
1. Push your customized template to a GitHub repository
2. Go to Settings > Pages
3. Select source branch (usually `main`)
4. Your site will be available at `https://username.github.io/repository-name`

### Netlify
1. Connect your GitHub repository to Netlify
2. Deploy automatically on every push
3. Get a custom domain (optional)

### Vercel
1. Import your repository to Vercel
2. Automatic deployments
3. Custom domain support

### Any Web Server
Simply upload the `index.html` file to any web server.

## Features Explained

### Dynamic Project Loading
- Fetches live data from GitHub API
- Shows stars, forks, and last updated date
- Falls back to cached data if API fails
- Graceful error handling

### Caching
- Projects data is cached for 24 hours
- Reduces API calls and improves performance
- Works offline after first load

### Responsive Design
- Works on desktop and mobile
- Terminal-style interface adapts to screen size
- Maintains readability on all devices

## Troubleshooting

### Projects Not Loading
- Check that your GitHub username and repository names are correct
- Ensure repositories are public
- Check browser console for API errors

### Styling Issues
- Verify all CSS is intact in the HTML file
- Check for conflicting stylesheets
- Test on different browsers

### Performance Issues
- The file should be around 13KB
- If significantly larger, check for added content
- Consider optimizing images if added

## Support

If you encounter issues:
1. Check the browser console for errors
2. Verify all placeholder text has been replaced
3. Ensure GitHub repositories are public
4. Test with a simple deployment first

## License

This template is MIT licensed. Feel free to modify and use for your own projects. 