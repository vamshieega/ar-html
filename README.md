# DeepAR Face Effect Web App

A production-ready web-based AR face effect application using DeepAR SDK, optimized for Netlify deployment.

## 🚀 Quick Start

### Local Development
```bash
npx serve
```
Then open: `http://localhost:3000/index.html`

### Netlify Deployment

1. **Connect your repository to Netlify**
   - Go to [Netlify](https://www.netlify.com/)
   - Click "New site from Git"
   - Connect your repository

2. **Deploy Settings**
   - Build command: (leave empty - static site)
   - Publish directory: `.` (root)
   - The `netlify.toml` file is already configured

3. **That's it!** Your app will be live automatically.

## 📁 Project Structure

```
AR-html/
├── index.html              # Main application file
├── netlify.toml           # Netlify configuration
├── assets/
│   ├── flower_face.deepar
│   ├── burning_effect.deepar
│   ├── Elephant_Trunk.deepar
│   ├── Emotion_Meter.deepar
│   ├── Emotions_Exaggerator.deepar
│   ├── Fire_Effect.deepar
│   ├── Humanoid.deepar
│   └── Neon_Devil_Horns.deepar
└── README.md
```

## 🎭 Features

- **8 AR Face Effects** - Select from multiple effects
- **Real-time Face Tracking** - Powered by DeepAR SDK
- **Responsive Design** - Works on desktop and mobile
- **Production Ready** - Optimized for deployment

## ⚠️ Requirements

- **DeepAR License Key** - Update `DEEPAR_LICENSE_KEY` in `index.html`
- **HTTPS** - Required for camera access (Netlify provides this automatically)
- **Modern Browser** - Chrome, Firefox, Safari, or Edge

## 🔑 License Key

1. Get a license from: https://www.deepar.ai/
2. Update the `DEEPAR_LICENSE_KEY` constant in `index.html` (line ~446)
3. Make sure your Netlify domain is included in your license

## 📝 Notes

- Effect files are automatically loaded from the `assets/` folder
- DeepAR SDK loads from CDN (requires internet connection)
- All effects use `.deepar` format (face effects only)
- GLB files (3D models) are not supported for face effects

## 🐛 Troubleshooting

### Camera Not Working
- Make sure you're using HTTPS (Netlify provides this)
- Allow camera permissions when prompted
- Check browser console for errors

### Effects Not Loading
- Verify effect files exist in `assets/` folder
- Check browser Network tab for 404 errors
- Ensure DeepAR license is valid for your domain

### License Errors
- Verify your license key is correct
- Make sure your Netlify domain is whitelisted in your DeepAR license
- Check console for specific error messages

## 📄 License

This project uses DeepAR SDK which requires a valid license. See https://www.deepar.ai/ for licensing information.
