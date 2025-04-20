# CS 203: Software Tools & Techniques for AI  
**IIT Gandhinagar**  
**Sem-II - 2024-25**

---

## LAB 11  
**Lead TA**: Himanshu Beniwal

**Total marks**: 100  
**Submission deadline**: Sunday, 20/04/2025 11:59 PM  

### Submission guidelines:
- Code should be added to a GitHub repository, and the repository details should be shared in the pdf.
- Submit the PDF showing screenshots of all steps involved in the following code.

> **Note**: Submitting this assignment solution confirms that you will follow the IITGN's honor code. We shall strictly penalize the submissions containing plagiarized text/code.

---

## Objective:
This assignment aims to learn about model quantization.

---

### 1. Dataset Preparation (10%)
- Load the training dataset and test data.
- Use 20% of the training dataset as the validation set.

---

### 2. Construct a Multi-Layer Perceptron (MLP) model. (10%)
- The parameter should be with:  
  `hidden_sizes=[512, 256, 128, 64]`
- Output should have two labels.
- With the following architecture:

- Count the number of trainable parameters in the model using the automated function (reference).

---

### 3. Train the model with 10 epochs and create the best-performing model (`checkpoint.pt`) (10%)
- Plot the validation accuracy + loss (epochs vs accuracy-loss).

---

### 4. Now use:
- **Dynamic Quantization with INT4 or INT8** [Link: here] (20%)  
  Use the `torch.quantization.quantize_dynamic()`

- **Half precision** (20%)  
  Use the `.half()` function. [Reference: here]

---

### 5. Fill the table for different quantization techniques. (30%)

| S.I. | Model Name | Accuracy (Out of 100) | Storage (In MB) | Inference time (In ms) |
|------|------------|------------------------|------------------|--------------------------|
| 1.   | Original   |                        |                  |                          |
| 2.   | Dynamic    |                        |                  |                          |
| 3.   | Half       |                        |                  |                          |
