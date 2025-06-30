# GarbageSort++
# ♻️ GarbageSort+ | Smart Waste Classifier & Eco-Score Analyzer

GarbageSort+ is a smart, AI-powered web application that helps users identify and classify garbage into six categories—**cardboard, paper, glass, metal, plastic, and trash**—using image recognition and deep learning. It also provides an **eco-score** to assess the recyclability of the waste item, making it ideal for sustainability education, smart city projects, and environmental research.

![GarbageSort+ Preview](https://github.com/yourusername/garbagesortplus/assets/preview.gif)

---

## Features

-  **Upload Image:** Classify waste items using AI
- 🏷 **Multi-task Learning:** Predict waste type & eco-score simultaneously
-  **Grad-CAM Heatmap:** Visualize what the model focuses on
-  **Download Results:** Export predictions to CSV
-  **Beautiful UI:** Fully responsive web interface with toggling sections and vibrant design

---
## Model Details

- **Backbone:** ConvNeXtTiny pretrained on ImageNet
- **Outputs:**
  - `class_output`: Waste type classification (sparse categorical crossentropy)
  - `eco_output`: Recyclability score prediction (mean squared error)
- **Training:**
  - Input Size: 224x224
  - Augmented with Keras `ImageDataGenerator`
  - Dual-output with custom Keras `Sequence`

---

## 🖼 Sample Usage

1. Go to the [GarbageSort+ App](https://your-hosted-app-link)
2. Upload a waste image
3. View:
   -  Waste category
   - Eco-score (0 to 1)
   -  Grad-CAM explanation
4.  Download CSV report

---

##  Recycling Ideas

-  Cardboard → Drawer organizers, compost
- 🗞 Paper → Recycled stationery, packaging
-  Metal → Garden tools, art projects
-  Plastic → DIY planters, 3D printing filaments
-  Glass → Decorative bottles, candle holders

---

## 🛡 Rules & Permissions

-  Upload only single, clear images of waste items
-  No sensitive, personal, or copyrighted images
-  All images are processed securely and discarded immediately
-  Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md)

---

##  Folder Structure

