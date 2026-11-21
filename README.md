# Through Studio — Online Color Grader for Photos & Video

**Through Studio** is a browser-based color grading tool with 370+ presets, custom filter extraction, and professional adjustment controls. Upload any photo or video, apply cinematic looks, fine-tune with manual sliders, and export your result — all in the browser, no server processing required.

## Live Demo
🔗 https://throughstudio.vercel.app/#/studio

## Features

### 370+ Preset Library
Curated preset packs organized by category:
- **Culture & Travel**: Kyoto, Santorini, Bali, Iceland, Sahara, Marrakech, and more
- **Film Stocks**: Kodak Gold, Fuji Pro, CineStill 800T, Portra, Tri-X, and 20+ film emulations
- **Cinematic Moods**: Cyberpunk, Noir, Anamorphic, Cyber Dystopia, Neo-Noir, and 30+ cinematic looks
- **Skin Tones**: Warm, Glow, Fresh Plate, Natural Thang, Baddie, and portrait-focused presets
- **Vintage & Retro**: VHS, 90s Vibe, Polaroid, Film Diary, Retro VHS, and analog emulations
- **Nature & Landscape**: Mountain Air, Forest Mist, Ocean Blue, Desert Sun, and scenic looks
- **Urban & Street**: Night Vibes, Chicago Loop, Penn Station, Tokyo Drift, and city looks

Each preset has 4 variants: Base, Deep, Bright, Vivid.

### Manual Adjustment Panel
Fine-tune any image with full manual controls:
- Exposure, Contrast, Highlights, Shadows, Whites, Blacks
- Temp (cool ↔ warm), Tint (green ↔ magenta)
- Saturation, Vibrance
- Film Grain, Sharpen, Vignette

### Filter Extraction & Import
- **Extract Filter**: Pull a color grade from any image and save it as a reusable filter
- **Import .XMP**: Load Lightroom-compatible .XMP preset files directly into the editor
- **Save Filter**: Save your custom grades for reuse later
- **Export**: Download your graded image

### Additional Tools
- Upload your own photos
- Sample gallery (Hollywood Palms, Glenfinnan Viaduct, Cliffs of Moher, Chongqing, Kyoto, Yamanote Line, and more)
- Cinema View mode for immersive editing
- Built-in music player with soundtracks

## Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React / Vanilla JS |
| Styling | CSS |
| Image Processing | Canvas API |
| Deployment | Vercel |

## How It Works

1. User uploads an image → rendered to `<canvas>`
2. Preset applied → color transformation runs on canvas pixels
3. Manual sliders adjust → real-time re-render of canvas
4. Extract Filter → samples dominant colors from image
5. Export → canvas.toDataURL() triggers browser download

## What I Learned

- How color spaces work (RGB, HSL, HSV)
- Canvas pixel manipulation for real-time image processing
- Building preset systems that apply consistent color transformations
- Client-side file handling (upload, export, localStorage)
- Deploying a static frontend on Vercel

## What I'd Improve Next

- [ ] Video color grading (currently photo-focused)
- [ ] Batch processing for multiple images
- [ ] User accounts to save filters across devices
- [ ] Before/after comparison slider
- [ ] Undo/redo history
- [ ] Mobile-responsive preset grid
- [ ] Keyboard shortcuts for common actions

## License

MIT License — feel free to use and modify.

## About the Author

**Harsh** — Class 9 student, aspiring AI/ML engineer, IMO math aspirant.

- Portfolio: https://throughharshlens.ai.studio
- GitHub: https://github.com/barveharsh1234-droid