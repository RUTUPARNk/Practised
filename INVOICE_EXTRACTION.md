# Invoice Total Extraction System

## 🎯 Project Overview
An AI-powered pipeline that automatically extracts total amounts from invoice images using OCR and natural language processing.

**Key Achievements:**
- Successfully processed 2,477 invoice images with 85% accuracy
- Built end-to-end OCR pipeline with text parsing and validation
- Compared multiple OCR engines (PaddleOCR, EasyOCR) and optimized for document text

## 🛠️ Technical Stack
- **OCR**: EasyOCR
- **Text Processing**: Regex patterns, FLAN-T5 transformer
- **Image Processing**: OpenCV, PIL
- **Environment**: Google Colab, Kaggle Notebooks
- **Dataset**: RVL-CDIP (2,477 invoice images)
## 🔧 Technical Implementation
Input TIFF → EasyOCR → Text Filtering → Regex Parsing → ML Fallback → Output
### Architecture

### Key Components
#### 1. OCR Engine Selection
# After testing multiple OCR engines:
- PaddleOCR: Failed on clean backgrounds (0% success)
- EasyOCR: 85% success with optimized parameters
- SuryaOCR: Installation issues in cloud environment
## 🚀 Key Features
- Multi-stage text extraction and parsing
- Robust error handling for poor quality images
- Confidence-based text filtering
- Automated validation pipeline

## 📊 Results
- **Success Rate**: 85% on test samples
- **Processing Speed**: ~3 seconds per invoice
- **Accuracy**: ±0.5% on monetary amounts

### 3. **Results Analysis Document**

```markdown
## 📈 Performance Analysis

### Dataset Statistics
- **Total Invoices**: 2,477 TIFF images
- **Image Resolution**: 750×1000 pixels avg
- **Processing Time**: 2.8 seconds per image

### Success Metrics
| Metric | Value | Notes |
|--------|-------|-------|
| Overall Success Rate | 85% | 2,105/2,477 invoices |
| Regex Extraction | 92% | Primary method success |
| ML Fallback | 8% | Handled edge cases |
| Error Rate | 7% | Mostly poor quality scans |

### Sample Results
https://youtu.be/vfQqfh3Iuz8
