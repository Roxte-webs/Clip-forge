# ClipForge AI — Mobile Video Editor MVP

This is a **working starter project**, not a full CapCut/After Effects replacement. It is designed to be easy to run from a mobile browser and progressively expand.

## Included in this MVP
- Mobile-first responsive interface
- Import one video file
- Preview using canvas
- Trim start/end range
- Playback speed controls
- Aspect ratio presets (16:9, 9:16, 1:1)
- Zoom
- Color-look presets
- Caption overlay and styles
- Cut-marker lane
- Load background music and preview it
- Volume controls
- Local project settings export as JSON
- Export selected trim as WebM using browser MediaRecorder (browser support varies)
- AI-style editing plan generator (local preset/rule based)
- Starter script generator
- Web Speech API live dictation where supported
- Installable PWA shell and basic offline caching

## Not yet included
- Real generative AI analysis of footage
- Automatic transcription of imported video audio
- Automatically generated cut decisions applied to a multi-clip timeline
- Full multi-track timeline editing
- Advanced AI denoising
- Voice cloning or voice generation
- Automatic meme/SFX asset selection
- Beat detection, motion tracking, masks, keyframes, compositing, or advanced effects
- Guaranteed export audio/music mixing; browser capture support varies

These are separate development milestones. No external AI API key is required for this MVP.

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a modern browser. For best PWA/export support, use a local web server or static host.
3. Import a video and test the controls.

## GitHub mobile workflow
1. Create a repository on GitHub.
2. Upload all files from this ZIP (not the ZIP itself, unless you prefer to keep it as an archive).
3. Open the repository in GitHub Codespaces if available on your account.
4. In the terminal, run:
   ```bash
   python3 -m http.server 8000
   ```
5. Open the forwarded port in the browser preview.
6. Keep your Codespace usage within the free allowance. GitHub currently documents 120 core hours/month and 15 GB storage for personal Free accounts; quotas/availability can change.

## Static hosting
The app is a static site. GitHub Pages or another static host can serve it. Exporting large videos happens in the user's browser; the app does not upload media to a server.

## Privacy
Imported video and music are processed in the browser. This starter does not upload your media. Speech recognition, if enabled by the browser, may use browser/provider services and is not guaranteed to be local.

## Roadmap
1. Multi-clip timeline with draggable clips and ripple edits.
2. Caption file import/export and Whisper-style transcription integration.
3. AI highlight detection using audio energy, scene changes, and user-defined signals.
4. Automatic edit decisions with editable timeline.
5. SFX/music library with license metadata.
6. Advanced filters, keyframes, transitions, masking and audio tools.
7. Optional local AI models and server-side processing when suitable free resources exist.
