# Skin Aging Predictor Application
![image](https://github.com/RH0627/skin_aging_predictor_app/blob/master/gui.png)
## Installation Guide

### Method 1: Using Git Clone
```bash
git clone https://github.com/RH0627/skin_aging_predictor_app.git
```

### Method 2: Direct Download
If Git clone is too slow, you can directly download these three files and extract `predictor.zip`:
- predictor.zip
- predictor.z01
- predictor.z02

## User Guide

### Important Notes
> ⚠️ **Note**: This software is large in size and may take some time to start. Please be patient. Thank you for using our software!
> 
> If the software doesn't respond when double-clicked, please try a few more times.

### Test Sequence
You can use the following peptide sequence to test the single sequence prediction function:
```
AAAAAE
```

### Environment Configuration
If you encounter a "Nonetype" error, this may be due to missing environment configuration. Please follow these steps:

1. Copy the `torch` folder to your `.cache` folder
2. `.cache` folder location:
   ```
   C:/Users/your_computer_name/.cache
   ```
3. If you can't find the `.cache` folder, click the 'predict' button once, and the folder will be automatically generated

## Common Error Solutions

### 1. Batch Processing Error '?'
- **Cause**: Input sequence file is too large or too many peptides
- **Recommendations**:
  - Process no more than 100 sequences per batch
  - Each sequence should not exceed 20 amino acids
  - For longer sequences, please use single sequence prediction

### 2. Input Prompt Error
- **Error Message**: "Please select file as CSV" or "Please enter the sequence"
- **Cause**: Program failed to correctly read user input
- **Solution**: Re-enter the batch file or single sequence

### 3. User Input Error
- **Error Message**: 'User input'
- **Cause**: Input sequence contains illegal characters (numbers, symbols, etc.)
- **Solution**: Ensure input contains only the 20 common amino acid abbreviations

### Batch File Format Requirements
> ⚠️ **Important**: When using a CSV file for batch processing, make sure the input column header is "Sequence"