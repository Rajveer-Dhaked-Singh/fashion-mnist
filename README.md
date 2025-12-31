# Fashion MNIST Classification using PyTorch

##  Project Overview
This project implements a **fully connected neural network (ANN)** using **PyTorch** to classify images from the **Fashion-MNIST dataset**.  
The dataset contains grayscale images of clothing items belonging to **10 classes**.

---

##  Dataset
- **Dataset Name:** Fashion-MNIST  
- **File Used:** `fashion-mnist_train.csv`

### Dataset Structure
- Column 0 → Class label (0–9)
- Columns 1–784 → Pixel values (28×28 image)

### Class Labels
| Label | Category |
|------|---------|
| 0 | T-shirt/top |
| 1 | Trouser |
| 2 | Pullover |
| 3 | Dress |
| 4 | Coat |
| 5 | Sandal |
| 6 | Shirt |
| 7 | Sneaker |
| 8 | Bag |
| 9 | Ankle boot |

---

##  Technologies Used
- Python
- PyTorch
- Pandas
- Scikit-learn
- Matplotlib

---

##  Model Architecture
Input (784)
→ Linear(128) + ReLU
→ Linear(64) + ReLU
→ Linear(10)


---

##  Project Workflow
1. Load Fashion-MNIST CSV file
2. Visualize first 16 images
3. Train-test split (80% / 20%)
4. Normalize pixel values
5. Create custom PyTorch Dataset
6. Load data using DataLoader
7. Define neural network model
8. Train model using SGD optimizer
9. Evaluate accuracy on test data

---

##  Hyperparameters
| Parameter | Value |
|---------|------|
| Learning Rate | 0.1 |
| Optimizer | SGD |
| Loss Function | CrossEntropyLoss |
| Batch Size | 32 |
| Epochs | 100 |
| Random Seed | 42 |

---

##  Training
During training, the average loss per epoch is printed:
epoch:1,loss:0.6443
epoch:2,loss:0.4321
epoch:3,loss:0.3867
epoch:4,loss:0.3573
epoch:5,loss:0.3385
epoch:6,loss:0.3233
epoch:7,loss:0.3078
epoch:8,loss:0.2976
epoch:9,loss:0.2843
epoch:10,loss:0.2745
epoch:11,loss:0.2655
epoch:12,loss:0.2602
epoch:13,loss:0.2530
epoch:14,loss:0.2434
epoch:15,loss:0.2393
epoch:16,loss:0.2331
epoch:17,loss:0.2282
epoch:18,loss:0.2222
epoch:19,loss:0.2177
epoch:20,loss:0.2112
epoch:21,loss:0.2039
epoch:22,loss:0.2011
epoch:23,loss:0.1997
epoch:24,loss:0.1942
epoch:25,loss:0.1881
epoch:26,loss:0.1855
epoch:27,loss:0.1813
epoch:28,loss:0.1759
epoch:29,loss:0.1717
epoch:30,loss:0.1695
epoch:31,loss:0.1643
epoch:32,loss:0.1655
epoch:33,loss:0.1575
epoch:34,loss:0.1566
epoch:35,loss:0.1532
epoch:36,loss:0.1480
epoch:37,loss:0.1522
epoch:38,loss:0.1453
epoch:39,loss:0.1476
epoch:40,loss:0.1426
epoch:41,loss:0.1370
epoch:42,loss:0.1341
epoch:43,loss:0.1336
epoch:44,loss:0.1277
epoch:45,loss:0.1281
epoch:46,loss:0.1241
epoch:47,loss:0.1234
epoch:48,loss:0.1265
epoch:49,loss:0.1188
epoch:50,loss:0.1168
epoch:51,loss:0.1169
epoch:52,loss:0.1156
epoch:53,loss:0.1106
epoch:54,loss:0.1090
epoch:55,loss:0.1089
epoch:56,loss:0.1036
epoch:57,loss:0.1042
epoch:58,loss:0.1039
epoch:59,loss:0.1012
epoch:60,loss:0.1019
epoch:61,loss:0.1044
epoch:62,loss:0.1016
epoch:63,loss:0.0963
epoch:64,loss:0.0954
epoch:65,loss:0.0947
epoch:66,loss:0.0950
epoch:67,loss:0.0899
epoch:68,loss:0.0923
epoch:69,loss:0.0895
epoch:70,loss:0.0851
epoch:71,loss:0.0858
epoch:72,loss:0.0881
epoch:73,loss:0.0826
epoch:74,loss:0.0836
epoch:75,loss:0.0829
epoch:76,loss:0.0861
epoch:77,loss:0.0818
epoch:78,loss:0.0808
epoch:79,loss:0.0792
epoch:80,loss:0.0736
epoch:81,loss:0.0752
epoch:82,loss:0.0792
epoch:83,loss:0.0766
epoch:84,loss:0.0776
epoch:85,loss:0.0739
epoch:86,loss:0.0709
epoch:87,loss:0.0694
epoch:88,loss:0.0734
epoch:89,loss:0.0631
epoch:90,loss:0.0687
epoch:91,loss:0.0627
epoch:92,loss:0.0641
epoch:93,loss:0.0701
epoch:94,loss:0.0628
epoch:95,loss:0.0727
epoch:96,loss:0.0623
epoch:97,loss:0.0591
epoch:98,loss:0.0570
epoch:99,loss:0.0639
epoch:100,loss:0.0656


---

##  Evaluation
The final evaluation metric is **accuracy** on the test dataset:
0.8824166666666666

---

## ▶️ How to Run
### 1. Install dependencies
```bash
pip install torch pandas scikit-learn matplotlib

