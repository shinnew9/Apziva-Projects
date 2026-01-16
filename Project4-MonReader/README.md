# Project 4

## Essence
**Accessibility-Focused OCR & Text-to-Speech Pipeline**

## Objective
- Extract text from large batches of images
- Filter unreliable OCR outputs using confidence thresholds
- Convert validated text into speech for accessibility

## Architecture
- Image Ingestion
  - Batch loading of image files containing textual content
- Image Preprocessing
  - Basic resizing and normalization to improve OCR robustness
- Optical Character Recognition (OCR)
  - Text extraction using EasyOCR
  - Generation of text segments with associated confidence scores
- Confidence-Based Filtering
  - Removal of low-confidence OCR outputs based on thresholding
  - Reduction of noisy or partially recognized text
- Text Aggregation & Normalization
  - Merging filtered text segments
  - Cleaning formatting artifacts for downstream processing
- Text-to-Speech (TTS)
  - Conversion of validated text into audio using Google Text-to-Speech (gTTS)
- Output Generation
  - Audio files representing extracted textual content for end users

 <br>
  ```
  
    flowchart LR    
      A[Image Files] --> B[Image Preprocessing]
      
      B --> C[OCR Engine<br/>(EasyOCR)]
      C --> D[Text + Confidence Scores]
      
      D --> E[Confidence-Based Filtering]
      E --> F[Text Aggregation & Normalization]

      F --> G[Text-to-Speech<br/>(gTTS)]
      G --> H[Audio Output Files]
    
    ```
 
  
## Key Points
- Clearly separates text extraction from quality control and audio generation
- Emphasizes that output quality is driven by pipeline design, not OCR alone
- Demonstrates a modular architecture that is easy to extend or replace components
