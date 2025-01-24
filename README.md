# 🌕 Automatic Detection of Craters and Boulders on the Lunar Surface  

### 🚀 **Overview**  
This project utilizes advanced computer vision techniques to automatically detect and segment craters and boulders on the lunar surface. By leveraging a **Mask R-CNN model**, the system performs precise instance segmentation, aiding lunar exploration and research.  

---

## 🛠️ **Features**  
- **Crater and Boulder Detection:** Identifies and segments craters and boulders with high accuracy.  
- **Instance Segmentation:** Generates masks directly over the original images.  
- **Custom Annotations:** Uses labeled datasets tailored for lunar surface analysis.  
- **Scalable Model:** Fine-tuned **Mask R-CNN** (COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x) for lunar-specific data.  

---

## 📂 **Repository Structure**  
```plaintext  
├── data/  
│   ├── annotations/      # COCO-format and NDJSON files  
│   ├── images/           # Raw and processed lunar images  
├── models/  
│   ├── mask_rcnn/        # Pretrained and fine-tuned model weights  
├── notebooks/  
│   ├── data_preparation.ipynb  # Data preprocessing and annotation conversion  
│   ├── training.ipynb          # Model training and evaluation  
│   ├── inference.ipynb         # Running predictions on new images  
├── results/  
│   ├── predictions/      # Visualized predictions and segmented masks  
├── requirements.txt      # Python dependencies  
├── README.md             # Project documentation  
└── LICENSE               # License information  
```  

---

## 🔬 **How It Works**  
1. **Data Annotation:**  
   - Images labeled using **Labelbox** and exported in COCO format.  

2. **Model Training:**  
   - Fine-tuned a pre-trained **Mask R-CNN** model using annotated datasets.  
   - Configured for two specific classes: **Crater** and **Boulder**.  

3. **Instance Segmentation:**  
   - Predictions include masks, labels, and bounding boxes, directly overlaid on input images.  

---

## 🚀 **Getting Started**  

### **1. Clone the Repository**  
```bash  
git clone https://github.com/Vanshdalal314/Automatic-detection-of-craters-and-boulders-on-lunar-surface.git  
cd Automatic-detection-of-craters-and-boulders-on-lunar-surface  
```  

### **2. Install Dependencies**  
Ensure you have Python 3.8+ installed. Then, run:  
```bash  
pip install -r requirements.txt  
```  

### **3. Run Training or Inference**  
- **Train the Model:**  
  Open and run `notebooks/training.ipynb` to train the model with the annotated dataset.  
- **Make Predictions:**  
  Use `notebooks/inference.ipynb` to test the model on new images.  

---

## 📊 **Results**  
- **Model Performance:**  
   Achieved high detection accuracy for craters and boulders with fine-tuned Mask R-CNN.  

- **Visualization:**  
   Predictions are overlaid on original images for clear interpretation.  
   Example:  
   ![Sample Output](results/predictions/sample_output.png)  

---

## 📜 **Future Work**  
- Enhance detection accuracy for smaller craters and boulders.  
- Experiment with other segmentation models (e.g., **UNet**).  
- Integrate the solution into larger planetary exploration systems.  

---

## 🤝 **Contributing**  
Contributions are welcome! Please fork the repository, make your changes, and submit a pull request.  

---

## 🌌 **Contact**  
For questions or collaborations:  
📧 **Email:** vanshdalal@example.com  
🔗 **LinkedIn:** [Your LinkedIn Profile](#)  

---

📌 **License:** This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.  

--- 

**Explore. Detect. Contribute.** 🚀
