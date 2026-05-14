---
name: vision-analyzer-v6
description: "VISION MODE: Activate ONLY when user says exactly 'Vision ON'. Supports multi-language (English + Romanian). Once active: ALWAYS auto-analyzes the body image at initiation, displays ALL measurements/proportions/sizes in cm BEFORE first command, then lists all abilities + how to run them. Stay active until 'Vision OFF'. Provides full VisionAnalyzerV6 v2.7 for 3D body reconstruction, anatomical landmarks, metric measurements, body_part_sizes_cm report, proportions and automatic detailed reports."
---

# Vision Analyzer V6 Ultimate – Interactive Mode (Multi-Language)

## Activation Rules (STRICT)
- **Activate ONLY** when the user writes **exactly** "Vision ON" (case insensitive).
- **Deactivate immediately** when the user writes **exactly** "Vision OFF".
- While active, this skill controls all vision/analysis responses.
- Multi-language support: Respond in **English** or **Romanian** depending on the user's language.

## After Activation (Mandatory Flow)
**IMPORTANT:** Upon activation with an image, the skill **ALWAYS** performs real body analysis immediately and displays the COMPLETE REAL measurements report **BEFORE** the first user command.

See full details in the original skill documentation.

## How to Use the Analyzer

```python
from scripts.vision_analyzer_v6 import VisionAnalyzerV6

analyzer = VisionAnalyzerV6()
body_data = analyzer.reconstruct_3d(image_path="your_image.jpg")
print(analyzer.get_body_part_sizes())
print(analyzer.get_body_proportions())
```

## Key Capabilities

1. High-Precision 3D Body Reconstruction
2. Extended Anatomical Landmark Detection
3. Complete Metric Measurements (in cm)
4. Body Proportions Analysis (WHR, Golden Ratio, etc.)
5. Glute Projection Analysis
6. Protection Mask Generation
7. Experimental Volumetric Estimation

This skill is part of the Advanced Body Remodeling toolkit.