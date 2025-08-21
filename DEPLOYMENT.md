# Deployment Guide

This document provides instructions for deploying the Crisis Helpline website.

## Prerequisites

- Node.js (version 14 or higher)
- npm or yarn package manager
- Git

## Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/username/crisis-helpline.git
   cd crisis-helpline
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```

4. Open your browser and navigate to `http://localhost:3000`

## Production Deployment

### Netlify (Recommended)

1. Connect your GitHub repository to Netlify
2. Set build command: `npm run build`
3. Set publish directory: `build` or `dist`
4. Deploy automatically on push to main branch

### Vercel

1. Import your GitHub repository to Vercel
2. Configure build settings if needed
3. Deploy with automatic deployments enabled

### Manual Deployment

1. Build the project:
   ```bash
   npm run build
   ```

2. Upload the contents of the `build` directory to your web server

## Environment Variables

If your application uses environment variables, create a `.env` file:

```
REACT_APP_API_URL=your_api_url_here
REACT_APP_ANALYTICS_ID=your_analytics_id_here
```

## Domain Configuration

- Update the `homepage` field in `package.json` with your domain
- Configure DNS settings to point to your hosting provider
- Set up SSL certificate for HTTPS

## Monitoring

- Set up error tracking (e.g., Sentry)
- Configure analytics (e.g., Google Analytics)
- Monitor uptime and performance

## Troubleshooting

### Common Issues

1. **Build fails**: Check Node.js version and dependencies
2. **404 errors**: Ensure routing is configured correctly
3. **Slow loading**: Optimize images and enable compression

### Support

For deployment issues, please:
1. Check the documentation
2. Search existing GitHub issues
3. Create a new issue with detailed information

