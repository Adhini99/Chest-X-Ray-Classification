# Chest X-Ray Classification Using DenseNet121 & Swin Transformer – My Deep Learning Approach to Multi-Label Medical Diagnosis
🎯 Motivation:
As someone deeply interested in applying AI to healthcare, I took on the challenge of automating chest X-ray (CXR) analysis to assist in diagnosing conditions such as Cardiomegaly, Edema, and Pneumonia. Multi-label classification in this domain is especially tough due to overlapping symptoms and class imbalance, but it presents a rewarding opportunity to create real-world impact.

🔧 What I Built:
I designed and implemented a multi-label classification pipeline integrating:

✅ DenseNet121 – A robust CNN architecture that excels at feature reuse and efficient gradient flow.

✅ Swin Transformer – A hierarchical vision transformer that captures both global and local image context.

✅ Ensemble Optimization – Applied differential evolution to intelligently combine model outputs, boosting overall performance and robustness.

💡 Key Highlights:
📚 Dataset: Used the NIH Chest X-ray14 dataset with a balanced sample strategy (100 images per class) to address class imbalance.

⚙️ Loss Function: Developed a custom loss function incorporating margin-based penalties to better manage label imbalance.

🔥 Training Strategy: Leveraged mixed precision training (AMP), dynamic learning rate scheduling with ReduceLROnPlateau, and early stopping for efficiency and stability.

🎯 Optimization: Fine-tuned ensemble weights using differential evolution (resulting in ~12% weight for DenseNet and ~88% for Swin Transformer).

📈 Results:
Test Mean AUC: 0.6268

Top Class Performance: Hernia (AUC: 0.86), Edema (0.77), Cardiomegaly (0.74)

🧪 ROC curves were also visualized to interpret model performance across labels.

💻 Tools & Libraries Used:
PyTorch, TIMM (for Swin Transformer), OpenCV, Pandas, Seaborn, Scikit-learn, and SciPy (for Differential Evolution).

🙌 Impact:
This project is a step toward empowering radiologists with automated diagnostic tools. By combining CNN and transformer-based models, I aimed to build a system that’s not just accurate but generalizable, scalable, and helpful in real clinical settings.
