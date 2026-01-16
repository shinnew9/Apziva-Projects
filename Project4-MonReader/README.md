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

</br>
  
## Key Points
- Clearly separates text extraction from quality control and audio generation
- Emphasizes that output quality is driven by pipeline design, not OCR alone
- Demonstrates a modular architecture that is easy to extend or replace components

</br>

## Insights
### OCR Reliability & Data Quality
  - OCR outputs varied significantly depending on image quality, layout, and font styles
  - Raw OCR results contained noisy or partially incorrect text that required post-processing
  - Confidence scores proved essential for distinguishing usable text from unreliable outputs

### Importance of Confidence-Based Filtering
  - Applying a confidence threshold improved overall output quality without manual review
  - Filtering reduced downstream errors propagated to the text-to-speech stage
  - Simple heuristics at the pipeline level had a larger impact than model complexity

### Pipeline Design Considerations
  - Batch processing enabled scalable handling of large image collections
  - Modular pipeline design allowed independent tuning of OCR, filtering, and TTS components
  - Clear separation of stages improved debuggability and extensibility

### Accessibility-Oriented Perspective
  - Converting extracted text into speech expanded usability for visually impaired users
  - Audio output provided an alternative interface for consuming image-based information
  - Accessibility goals influenced design decisions beyond pure OCR accuracy

### Practical Limitations
  - OCR performance degraded on low-resolution or highly stylized images
  - Confidence thresholds required tuning based on data characteristics
  - Text-to-speech quality depended on OCR accuracy and text normalization

</br>

## Outcome
  - Built an end-to-end OCR and text-to-speech pipeline for batch image processing
  - Improved text extraction reliability through confidence-aware filtering
  - Demonstrated how lightweight pipeline design choices can significantly enhance usability

</br>

## Technologies Used
### Programming Language
  - Python
### Libraries & Tools
  - EasyOCR
  - Google Text-to-Speech (gTTS)
  - NumPy, pandas
### Pipeline Components
  - OCR processing
  - Confidence-based filtering
  - Text normalization
  - Audio generation

</br>

## 🧠 What I Learned
- OCR systems require explicit quality control mechanisms in real-world pipelines
- Confidence scores are critical signals for managing noisy model outputs
- Designing for accessibility often changes how success is defined in ML systems
- Simple, well-structured pipelines can outperform more complex designs in practice

</br>

## 🔮 Future Work
  - Explore alternative OCR engines for improved multilingual support
  - Introduce adaptive confidence thresholds based on image characteristics
  - Extend the pipeline with document layout analysis
  - Integrate real-time audio playback or user-facing interfaces
