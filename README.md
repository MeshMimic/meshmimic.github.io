# MeshMimic Website

This is the modified website for the MeshMimic paper, adapted from the "Hiking in the Wild" template.

## What Has Been Changed

### Content Replacements:
1. **Title**: Changed to "MeshMimic: Geometry-Aware Humanoid Motion Learning through 3D Scene Reconstruction"
2. **Authors**: Updated with all 23 authors and their affiliations (X-Humanoid, HKUST(GZ), HKU, Tsinghua, CUHK, SJTU, ANU)
3. **Abstract**: Replaced with MeshMimic abstract describing the framework for learning motion-terrain interactions from video
4. **BibTeX**: Updated citation information
5. **Videos**: Replaced all original videos with MeshMimic supplementary materials

### Layout Changes:
1. **Removed**: Hero background video section (as requested, since outdoor demo video is not ready)
2. **Removed**: YouTube embed section (as requested)
3. **Added**: Two new video sections:
   - **Real2Sim2Real Results**: Shows real-world videos paired with simulation reconstructions
     - Climb Box (3 pairs)
     - Jump Box (2 pairs)
     - Other Skills (2 pairs)
   - **Real2Sim Results**: Shows simulation-only results
     - Long Parkour Sequences (4 videos)
     - Short Parkour Skills (5 videos)

## File Structure

```
hiking-in-the-wild/
├── index.html                    # Main website file (modified)
├── index_original_backup.html    # Backup of original file
├── static/                       # CSS, JS, and other static files
│   ├── bulma.min.css
│   ├── index.css
│   ├── jquery.min.js
│   └── ...
├── resources/
│   ├── icon.png
│   ├── logo.png
│   ├── loading-icon.gif
│   ├── preview-cover.jpg
│   └── meshmimic_videos/        # Your video files
│       ├── real2sim2real_videos/
│       └── real2sim_videos/
└── README.md                     # This file
```

## How to Use

### Local Testing:
1. Extract the zip file
2. Navigate to the directory
3. Start a local web server:
   ```bash
   python3 -m http.server 8080
   ```
4. Open your browser and go to `http://localhost:8080`

### Deployment:
- Upload the entire `hiking-in-the-wild` directory to your web server
- Make sure all file paths remain relative
- The website should work immediately without any configuration

## Notes

- All video files are embedded using HTML5 `<video>` tags with autoplay, loop, and mute attributes
- Videos are organized by category for easy navigation
- The website is responsive and works on mobile devices
- Original template credits are maintained in the footer

## Video Organization

### Real2Sim2Real Videos (14 videos total):
- Each skill shows a pair: real-world video + simulation reconstruction
- Demonstrates the pipeline from real human motion to robot simulation

### Real2Sim Videos (9 videos total):
- Shows various parkour skills in simulation
- Includes both long sequences and short skill demonstrations

## Future Updates

When you have additional materials ready:
1. **Outdoor demo video**: Can be added as a hero background video at the top
2. **YouTube video**: Can be embedded in a dedicated section
3. **Paper PDF**: Update the "Paper" link to point to your PDF file
4. **arXiv link**: Update when your paper is published on arXiv
5. **Code repository**: Update the "Code" link to point to your GitHub repository

## Contact

For questions or modifications, please refer to the original paper authors.
