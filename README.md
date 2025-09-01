# The Mountains of Madness

Interactive demos exploring procedural terrain generation algorithms through pure JavaScript implementations. From basic Perlin noise to advanced multifractal techniques, this project provides hands-on learning for game developers and computer graphics enthusiasts.

🏔️ **[Live Demo](https://amanpriyanshu.github.io/The-Mountains-of-Madness/)**

## Overview

This project demonstrates six different approaches to procedural terrain generation, each building on the limitations of previous methods. All implementations are pure JavaScript with real-time parameter controls and performance analysis.

## Algorithms Implemented

### 1. [Basic Perlin Noise](simple-perlin.html)
The foundation of procedural terrain - smooth, continuous noise that transforms random values into rolling hills through gradient-based interpolation.

### 2. [Additive Perlin Noise](additive-perlin.html) 
Fractal terrain generation through layered octaves. Multiple noise functions at different scales combine to create natural-looking landscapes with both large formations and fine details.

### 3. [Multiplicative Perlin Noise](multiplicative-perlin.html)
Terrain masking through layer multiplication instead of addition. Creates dramatic erosion patterns and sharp terrain contrasts by using each layer as a selective filter.

### 4. [Domain Warping](domain-warping.html)
Coordinate space distortion applied before noise sampling. Warps the sampling coordinates themselves to create organic, flowing terrain patterns that break free from grid-like artifacts.

### 5. [Exponential Slope Weighting](exponential-weighting.html)
Post-processing technique that selectively smooths steep terrain areas while preserving gentle slopes. Useful for creating playable game terrain by eliminating knife-edge ridges.

### 6. [Ridged Multifractal](ridged-multifractal.html)
Mathematical transformation that inverts valleys into sharp ridges. Each octave's influence depends on previous results, creating dramatic alpine terrain with realistic detail distribution.

## Features

- **Interactive Parameter Controls**: Real-time adjustment of all algorithm parameters
- **Performance Monitoring**: Chunk-based generation timing and analysis
- **Chunked Generation**: Terrain generated in tiles for scalability and streaming
- **3D Visualization**: Isometric rendering with wireframe overlay
- **Mathematical Formulas**: Complete equations for each technique
- **Educational Content**: Detailed explanations of each algorithm's behavior

## Technical Details

- Pure JavaScript implementation (no external libraries)
- Seeded random generation for reproducible results
- Optimized for real-time parameter manipulation
- Responsive design with mobile support
- Modular architecture for easy algorithm comparison

## Performance Considerations

Each algorithm has different computational costs:
- **Basic Perlin**: 1x baseline cost
- **Additive**: Linear scaling with octave count (3-6x typical)
- **Multiplicative**: Similar to additive but dramatic visual impact per layer
- **Domain Warping**: 6-10x cost due to coordinate transformation requirements
- **Exponential Weighting**: Post-processing pass, minimal additional cost
- **Ridged Multifractal**: Variable cost based on spectral weighting complexity

## Applications

These techniques are applicable to:
- Game world generation
- Procedural content creation
- Computer graphics research
- Generative art projects
- Educational demonstrations of noise functions

## License

Apache 2.0 License - see [LICENSE](LICENSE) file for details.

## Author

**Aman Priyanshu**  
- Website: [amanpriyanshu.github.io](https://amanpriyanshu.github.io/)

This README focuses on the technical value while maintaining some personality through the subtitle. It provides clear navigation to each demo and emphasizes the educational aspects that make your project discoverable to developers looking for terrain generation resources.
