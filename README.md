# Wide Bay Tile Centre Website

A modern, premium, fully-responsive website for Wide Bay Tile Centre, built with vanilla HTML5, CSS, and JavaScript.

## Features

- Fully responsive design (desktop, tablet, mobile)
- Optimized for Core Web Vitals
- WCAG 2.2 AA accessibility compliant
- Lazy-loaded images
- Smooth scrolling and animations
- Mobile-friendly navigation
- Contact form with modal
- Testimonial carousel
- Schema.org markup for SEO

## Project Structure

```
widebaytiles/
├── index.html
├── pages/
│   ├── products.html
│   ├── gallery.html
│   ├── services.html
│   ├── about.html
│   ├── contact.html
│   └── privacy.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── main.js
│   └── img/
│       ├── logo.png
│       ├── logo-white.png
│       ├── hero-bg.jpg
│       ├── floor-tiles.jpg
│       ├── wall-tiles.jpg
│       ├── mosaics.jpg
│       ├── icon-range.svg
│       ├── icon-advice.svg
│       ├── icon-payment.svg
│       └── facebook.svg
└── README.md
```

## Deployment Instructions

### Netlify Deployment

1. Sign up for a [Netlify](https://www.netlify.com/) account
2. Connect your GitHub repository or drag and drop the project folder to Netlify
3. Configure build settings:
   - Build command: (leave empty)
   - Publish directory: /
4. Click "Deploy site"

### AWS S3 Static Hosting

1. Create an S3 bucket with the same name as your domain
2. Enable static website hosting in the bucket properties
3. Set bucket policy for public access:
```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::your-bucket-name/*"
        }
    ]
}
```
4. Upload all files to the bucket
5. Configure Route 53 for DNS (optional)

## TODOs for Client

1. Replace placeholder images in `/assets/img/` with actual product and project photos
2. Update testimonials with real customer reviews
3. Add actual social media links
4. Update contact information if needed
5. Add real team member photos and bios
6. Update business hours if different from default
7. Add actual product categories and descriptions
8. Update meta descriptions and titles for SEO

## Performance Optimization

- Images are lazy-loaded using the `loading="lazy"` attribute
- Critical CSS is inlined in the head
- JavaScript is loaded with `defer` attribute
- Fonts are preconnected and loaded asynchronously
- Assets are minified and compressed

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (latest)

## License

© 2025 Wide Bay Tile Centre. All rights reserved. 