# Personal Portfolio Site

A clean, responsive single-page portfolio website to showcase your projects and professional information.

## Features

- Responsive design that works on all devices
- Clean and modern UI
- Sections for About, Projects, and Contact
- Easy to customize and maintain
- Smooth scrolling navigation
- Project cards with tags and links

## How to Use

1. **Customize the Content**:
   - Open `index.html` and replace the placeholder content with your information
   - Add your own projects to the projects section
   - Update the social media links in the contact section

2. **Customize the Styling**:
   - The color scheme can be easily modified in the `:root` section of `styles.css`
   - Adjust spacing, fonts, and other styles as needed

3. **Add Your Own Images**:
   - Replace the placeholder images with your own project screenshots
   - Add a favicon if desired

## Deployment Options

### GitHub Pages (Free and Easy)

1. Create a GitHub repository for your site
2. Push your code to the repository
3. Go to Settings > Pages
4. Select the branch to deploy (usually `main`)
5. Your site will be available at `https://your-username.github.io/repository-name/`

For a custom domain:
1. In GitHub repository settings, under Pages, add your custom domain
2. Configure DNS settings with your domain provider (add A records and/or CNAME)

### Netlify (Free Tier Available)

1. Create an account on [Netlify](https://www.netlify.com/)
2. Connect your GitHub repository or drag and drop your site folder
3. Your site will be deployed automatically
4. You can set up a custom domain through Netlify

### Vercel (Free Tier Available)

1. Create an account on [Vercel](https://vercel.com/)
2. Connect your GitHub repository
3. Your site will be deployed automatically
4. Set up a custom domain through Vercel

## Updating Your Site

To add new projects or update existing content:

1. Edit the HTML file to add new project cards or update information
2. If you deployed through GitHub Pages, push changes to your repository
3. If using Netlify or Vercel, changes will automatically deploy when you push to your repository

## Maintenance

This is a static website, which means:
- No database or backend needed
- Very low maintenance requirements
- Fast loading times
- Very secure (no server-side code to exploit)

## Future Enhancements

Consider adding:
- A blog section
- Image gallery
- Dark/light mode toggle
- Contact form (would require a form submission handler) 