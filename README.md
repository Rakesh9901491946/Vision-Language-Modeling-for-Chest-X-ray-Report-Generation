# 🧠 Vision-Language Modeling for Chest X-ray Report Generation

This repository contains the codebase, training scripts, and documentation for our research project:  
**"Vision-Language Modeling for Chest X-ray Report Generation: A Cross-Domain Study Using MIMIC-CXR and IU Datasets"**

---

## 📌 Project Summary

This project explores an end-to-end vision-language model that generates clinically meaningful **Impression** sections from paired **frontal and lateral chest X-ray images**, optionally using **Findings** as prompts.

The architecture is a **two-view Vision Transformer (ViT)** encoder fused via **average pooling**, followed by a **BioBART encoder–decoder** conditioned on a **learned image prefix token**. The model is trained and evaluated on the **MIMIC-CXR** and **Indiana University (IU X-ray)** datasets.

---

## 🔍 Key Features

- ✅ **Two-view ViT encoding** for frontal & lateral image inputs.
- 🔗 **Average fusion** of [CLS] tokens from both views.
- 🧩 **Prefix projection** for image-text coupling into BioBART.
- 🧠 **BioBART decoder** generates section-aware clinical summaries.
- 🧪 **Clinical F1** used as the primary metric for evaluation.
- ♻️ Robust training loop with **staged unfreezing**, prompt conditioning, and inference controls.
- 🧰 Ready-to-run on **MIMIC-CXR** and **IU datasets**.

---

## 🧱 Architecture

![Architecture Diagram](Images/method_schematic.png)

---

## 📁 Repository Structure

