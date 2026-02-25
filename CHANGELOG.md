# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [2.0.0] - 2026-02-25

### Added

- Chromatic aberration post-processing effect
- Vignette shader darkening screen edges
- Reflective metallic floor synced with color cycle
- Emissive pulse breathing animation on structures
- CSS scanlines overlay with slow scroll animation
- Ghost structure (smaller echo offset behind main)
- Floating particles with additive blending
- Atmospheric fog (FogExp2) for depth
- Per-instance color variation based on tube height

### Changed

- Typography removed entirely, visual-only experience
- Tubes switched from CylinderGeometry to BoxGeometry for performance
- Grid reduced to 40×40 desktop / 24×24 mobile
- Chromatic aberration and vignette combined into single ShaderPass
- Film grain intensity increased to 0.25
- Structure height and position rebalanced

## [1.1.0] - 2026-02-25

### Changed

- Typography switched from League Gothic to Arial for a cleaner, more minimal look
- Title and link moved to top-left corner, white color
- Removed Google Fonts dependency
- Structure positioned lower in the scene for better framing
- Bloom parameters tuned separately for desktop and mobile to avoid overexposure
- Camera pulled back for more surrounding dark space

## [1.0.0] - 2026-02-25

### Added

- Immersive Three.js scene with instanced tube structure forming an abstract crystalline silhouette
- UnrealBloom post-processing for organic light diffusion
- Slow color cycling between electric blue, volcanic orange, dense violet, and deep ruby
- Automatic camera orbit with vertical oscillation
- Film grain overlay via Canvas 2D
- Minimal typography with League Gothic
- Responsive design with mobile performance optimizations
- Open Graph and Twitter Card meta tags
- Inline base64 favicon
