# Degaga's Portfolio Website

A modern, responsive portfolio website built with HTML5, CSS3, JavaScript, PHP, and MySQL.

## Features

- **Responsive Design**: Mobile-first approach using CSS Grid and Flexbox
- **Modern UI**: Clean and professional design with smooth animations
- **Interactive Elements**: JavaScript-powered interactions and form validation
- **Contact Form**: PHP-powered contact form with email functionality
- **Project Showcase**: Display your projects with descriptions and links
- **Skills Section**: Visual representation of your technical skills
- **Education Section**: Highlight your academic background

## Project Structure

```
my-portfolio-website/
├── index.html              # Home page
├── about.html              # About page
├── projects.html           # Projects showcase
├── contact.html            # Contact page
├── assets/
│   ├── css/
│   │   └── style.css       # Main stylesheet
│   ├── js/
│   │   └── main.js         # JavaScript functionality
│   └── php/
│       └── contact.php     # Contact form handler
└── README.md               # This file
```

## Setup Instructions

### 1. Local Development
1. Download/clone this project to your local machine
2. Open the project folder in your code editor
3. Use a local server (XAMPP, WAMP, or Live Server extension) to run the project
4. Navigate to `http://localhost/your-project-folder` in your browser

### 2. Email Configuration
To enable the contact form functionality:

1. **For Local Testing**: 
   - Use XAMPP/WAMP with PHP mail() function
   - Configure SMTP settings in your local environment

2. **For Production**:
   - Update the email address in `assets/php/contact.php` (line 25)
   - Configure your web server's mail settings
   - Consider using a service like SendGrid or Mailgun for better deliverability

### 3. Database Setup (Optional)
If you want to store contact form submissions in a database:

1. Create a MySQL database named `portfolio_db`
2. Create a `messages` table with the following structure:
   ```sql
   CREATE TABLE messages (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(100) NOT NULL,
       email VARCHAR(100) NOT NULL,
       subject VARCHAR(200) NOT NULL,
       message TEXT NOT NULL,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
   ```
3. Uncomment the database section in `assets/php/contact.php`
4. Update database credentials in the PHP file

## Customization

### Personal Information
Replace the placeholder content with your actual information:

1. **Home Page** (`index.html`):
   - Update name, title, and introduction
   - Replace profile placeholder with your photo

2. **About Page** (`about.html`):
   - Update bio and personal information
   - Modify education details
   - Adjust skill levels

3. **Projects Page** (`projects.html`):
   - Replace sample projects with your actual projects
   - Add real project images
   - Update GitHub and demo links

4. **Contact Page** (`contact.html`):
   - Update contact information
   - Modify email address in PHP file

### Styling
- Modify `assets/css/style.css` to change colors, fonts, and layout
- Update the color scheme by changing CSS variables
- Add your preferred fonts from Google Fonts

### Images
- Replace placeholder images with your actual photos
- Add project screenshots to the projects section
- Optimize images for web (use tools like TinyPNG)

## Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with Grid and Flexbox
- **JavaScript**: Interactive functionality and form validation
- **PHP**: Server-side form processing
- **MySQL**: Database storage (optional)
- **Font Awesome**: Icons
- **Responsive Design**: Mobile-first approach

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## Performance Tips

1. **Optimize Images**: Compress images before uploading
2. **Minify CSS/JS**: Use minified versions for production
3. **Enable Gzip**: Configure server compression
4. **Use CDN**: Consider using a CDN for static assets

## Security Considerations

1. **Form Validation**: Both client-side and server-side validation
2. **Input Sanitization**: All user inputs are sanitized
3. **CSRF Protection**: Consider adding CSRF tokens for production
4. **Rate Limiting**: Implement rate limiting for contact form

## Deployment

### Shared Hosting
1. Upload all files to your web server
2. Ensure PHP is enabled
3. Configure email settings
4. Test the contact form

### VPS/Dedicated Server
1. Set up web server (Apache/Nginx)
2. Install PHP and MySQL
3. Configure SSL certificate
4. Set up email server or use SMTP service

## Future Enhancements

- [ ] Add a blog section
- [ ] Implement a CMS for easy content management
- [ ] Add more interactive animations
- [ ] Create an admin panel for project management
- [ ] Add dark mode toggle
- [ ] Implement lazy loading for images
- [ ] Add SEO optimization
- [ ] Create a sitemap

## Support

If you encounter any issues or need help customizing the portfolio:

1. Check the browser console for JavaScript errors
2. Verify PHP configuration and email settings
3. Test the contact form functionality
4. Ensure all file paths are correct

## License

This project is open source and available under the MIT License.

---

**Happy Coding!** 🚀

Remember to replace all placeholder content with your actual information and customize the design to match your personal brand.
