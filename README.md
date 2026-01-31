# AR Menu

An interactive AR menu application that allows users to view 3D food models in augmented reality.

## Features

- 📱 Mobile AR support (iOS & Android)
- 🎨 Beautiful loading animation with progress indicator
- 🔄 Optimized 3D model for fast loading
- ✨ Smooth transitions and animations

## How to Use

1. Open the application on your smartphone
2. Wait for the model to load (you'll see a progress indicator)
3. Click "View in AR" button to place the dish in your space
4. Move your phone to position the 3D model on a surface

## Technical Details

- **3D Model**: Optimized GLB format (1.06 MB)
- **AR Framework**: Google Model Viewer
- **Supported Platforms**: iOS (AR Quick Look), Android (Scene Viewer)

## Local Development

To run locally:

```bash
npx -y http-server -p 8000
```

Then open `http://localhost:8000` in your browser.

## Troubleshooting

### AR Button Not Appearing

If the loading reaches 100% but the AR button doesn't appear:

1. **Open browser console** (F12 or right-click → Inspect → Console)
2. Look for console messages:
   - "Model loaded successfully!" - Model loaded correctly
   - "AR button should now be visible" - Button was shown
   - Any error messages about model loading

3. **Check the model file**:
   - Ensure `dish-optimized.glb` exists in the same directory
   - File size should be ~1.06 MB

4. **Browser compatibility**:
   - Use Chrome on Android or Safari on iOS for best AR support
   - Desktop browsers will show a message to use mobile

### Model Not Loading

If you see an error alert:
- Check that the GLB file path is correct
- Ensure the file is not corrupted
- Try using the original `dish.glb` file instead

## Files

- `index.html` - Main application
- `dish-optimized.glb` - Optimized 3D model (recommended)
- `dish.glb` - Original 3D model
- `image.webp` - Preview image for loading screen

## License

MIT
