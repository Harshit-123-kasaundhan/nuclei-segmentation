---

# **U-Net Nuclei Segmentation**  

## **Overview**  
This project implements a **U-Net-based architecture** for nuclei segmentation in microscopy images. The primary goal is to accurately identify and segment nuclei to aid in **biomedical research and analysis**.  

---

## **Features**  
- **U-Net Architecture**: Fully convolutional neural network optimized for biomedical image segmentation.  
- **Accurate Segmentation**: High precision and recall in identifying nuclei, even in complex backgrounds.  
- **Custom Dataset Support**: Seamlessly adapt the pipeline for new datasets.  

---

## **Getting Started**  
### **Prerequisites**  
This project is designed to run on **Google Colab** with the following setup:  
- **Python**: 3.11  
- **TensorFlow**: 2.17  

### **Dataset**  
1. Use the [Kaggle Nuclei Segmentation Dataset](https://www.kaggle.com/code/paultimothymooney/identification-and-segmentation-of-nuclei-in-cells/input) or your custom dataset.  
2. Place the **images** in the `data/images/` directory and the corresponding **masks** in the `data/masks/` directory.  

---

## **Model Architecture**  
The U-Net model comprises three key components:  

1. **Contracting Path**:  
   - Extracts image features using successive **convolutional layers** and **max-pooling**.  

2. **Bottleneck**:  
   - Acts as a bridge between the encoder and decoder.  

3. **Expanding Path**:  
   - Recovers spatial dimensions through **up-sampling** and **skip connections** for precise segmentation.  

---

## **Results**  
Here’s an example of the segmentation output: vall accuracy and train accuracy  

![Segmentation Example](https://github.com/user-attachments/assets/5df63382-b243-4a18-9983-f6d39084a343)  

---

## **References**  
- [Original U-Net Paper](https://arxiv.org/pdf/1505.04597v1)  

---  
