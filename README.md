# CareShareOCR

##  **Overview of OCR Prescription Chatbot**

###  **Need for the OCR Chatbot**

In many healthcare settings, especially in under-resourced or manual systems, prescriptions are still written by hand or printed without digital copies. This creates challenges in:

* **Understanding illegible handwriting**
* **Digitally storing and accessing prescriptions**
* **Extracting structured data like medicine names and dosages**
* **Reducing manual data entry errors**

Your **OCR chatbot** addresses these issues by **automatically reading and extracting important data** from prescription images, making medical workflows faster, accurate, and digital.

---

## ✨ **Features of the OCR Chatbot**

1. ** Prescription Image Upload**

   * Users can upload images of printed or handwritten prescriptions directly into the chatbot interface.

2. ** Automated Text Extraction**

   * Utilizes OCR (Optical Character Recognition) to recognize and convert image-based text into readable format.

3. ** Field Identification**

   * Extracts key details such as:

     * Patient Name
     * Age
     * Doctor’s Name
     * Date
     * Prescribed Medicines
     * Dosage Instructions

4. ** Preprocessing for Accuracy**

   * Enhances the image (grayscale, noise removal, contrast) before OCR to improve clarity and recognition.

5. ** Structured Output**

   * Outputs the data in an organized JSON/text format that can be saved or reviewed easily.

6. ** Integrated with Chatbot**

   * Combines OCR with your medical assistant chatbot, so users can both extract and inquire about prescriptions in the same interface.

---

##  **How It Extracts Data – Step-by-Step**

1. ** Image Input**

   * User uploads a prescription image (JPEG, PNG, etc.).

2. ** Image Preprocessing**

   * Converts the image to grayscale.
   * Applies noise reduction and sharpens text using OpenCV filters.
   * Improves contrast using thresholding techniques.

3. ** OCR Processing**

   * Passes the cleaned image to **Tesseract OCR**, which scans for readable text patterns and converts them into plain text.

4. ** Text Parsing (Optional Enhancement)**

   * Splits text lines and identifies patterns like:

     * “Name:” or “Rx:” or “Take 1 capsule…”
   * Maps these lines to predefined fields using rule-based or NLP techniques.

5. ** Output Generation**

   * Displays the extracted text in a readable format.
   * Optionally provides structured output (e.g., JSON or tables).

---

##  **Result**

Your OCR chatbot provides a **time-saving, accurate, and user-friendly solution** for digitizing prescriptions—especially helpful in clinical, pharmacy, or donation-based platforms like CareShare.

