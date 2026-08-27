---
layout: default
---


---

**Hotel Recommendation Using Hotel Images and Reviews**
---

* Technologies/Tools: Python, PyTorch, HuggingFace Transformers (RoBERTa), OpenAI/LAION CLIP, NumPy, Pandas, scikit-learn, Optuna, Matplotlib/Seaborn
* Github URL: [Project](https://github.com/sabbirshanto/Hotel-Recommendation-Using-Coattention-Model)
* Built a personalized hotel recommender that fuses text reviews and hotel images with a token–patch co-attention mechanism. Review tokens (RoBERTa) and image patches (CLIP) attend to each other to capture aspect cues (cleanliness, room quality, amenities). The user–item interaction is modeled with a lightweight ranking head optimized via BPR/LambdaRank-style objectives. The pipeline includes robust preprocessing (text cleaning, sentiment/aspect cues, image normalization), reproducible splits, and evaluation with Precision@K / Recall@K / NDCG@K / MAP@K.

**Plant Disease Classification with Transfer Learning and Explainable AI**
---
* Technologies/Tools: Python, TensorFlow/Keras, NumPy, Pandas, Matplotlib, scikit-learn, Gradio, Kaggle API
* Github URL: [Project](https://github.com/sabbirshanto/Plant-Disease-Classification-with-Transfer-Learning-and-Explainable-AI)
* Built an end-to-end image classification pipeline for plant leaf diseases using transfer learning. I created efficient tf.data loaders, applied light augmentations, and used EfficientNetB0 (ImageNet weights) with a warm-up phase and selective fine-tuning. Evaluation includes Accuracy/Top-3 Accuracy and a scikit-learn report (Precision/Recall/F1). For explainability, I generated Class Activation Maps (CAM) to highlight discriminative regions on leaves, and packaged a Gradio demo for quick inference.



**
## COVID-19 Big Data Analysis with PySpark**
---

* Technologies/Tools: PySpark (SparkConf, SparkContext, SQLContext, Spark SQL), HDFS (bdrenhdfs client), Python (logging, random), Pandas-style aggregations via Spark, Linux CLI
* Github URL: [Project](https://github.com/sabbirshanto/Covid-19-analysis-using-spark)
* Built a distributed data-processing job in PySpark to read COVID-19 case data from HDFS, normalize month fields to human-readable names, create a temporary SQL view, and compute InfectionRate and DeathRate per month–year–country. Results are coalesced to a single CSV  and written back to HDFS. The job is production-ready with logging, randomized backoff, and overwrite-safe output behavior.

**Diabetes Prediction Web App using Streamlit**
---

* Technologies/Tools: Python, Streamlit, scikit-learn (pretrained model via Rclf.pkl), NumPy, Pandas
* Github URL: [Project](https://github.com/sabbirshanto/Diabetes-Streamlit)
* Built a lightweight Streamlit app that loads a pretrained classifier from Rclf.pkl and predicts diabetes risk from four inputs—Glucose, Insulin, BMI, Age. The UI collects user values, calls classifier.predict([[Glucose, Insulin, BMI, Age]]), and shows a friendly result: “you don't have diabetes” for class 0 or “You have diabetes! Please consult with doctor.” for class 1.


**Phishing Email Detection with LLaMA**
---

* Technologies/Tools: Python, PyTorch, HuggingFace Transformers, PEFT (LoRA/QLoRA), bitsandbytes (4-bit), Datasets, scikit-learn, Pandas, Accelerate
* Github URL: [Project](https://github.com/sabbirshanto/Phishing-Email-Detection-with-LLaMA)
* Built a phishing classifier by instruction-tuning LLaMA with LoRA/QLoRA (4-bit) to keep VRAM/RAM low while preserving performance. The pipeline cleans raw emails (removes headers/trackers, normalizes URLs, lowercases where helpful), creates a compact prompt template (system + user = email text; assistant = label), tokenizes to a max context window, and trains with class-balanced sampling. Evaluation reports Accuracy / Macro-F1 / ROC-AUC with a confusion matrix and error analysis (typical false positives: marketing; false negatives: spear-phishing with benign tone).
