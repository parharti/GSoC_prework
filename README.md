# GSoC_prework
#  Multichannel Cell Candidate Detection – GSoC 2025 Prototype

This notebook demonstrates a prototype implementation of the **cell candidate detection pipeline** described in my GSoC 2025 proposal for the [Cellfinder](https://github.com/brainglobe/cellfinder) project under the **BrainGlobe** ecosystem.

---

##  Objective

To simulate and test **cell candidate detection** across an **arbitrary number of imaging channels** using synthetic brain-like data.

This serves as a foundational step toward enabling **multi-channel-aware classification** in Cellfinder, which is currently limited to 2 channels (signal + background).

---

##  What's Implemented

- ✅ Synthetic **3D brain image** loading (3 channels)
- ✅ Blob detection using `skimage.feature.blob_log` on:
  - Individual channels
  - Averaged combination of multiple channels
- ✅ Feature extraction: Blob **radius**
- ✅ **Z-score normalization** of features per channel
- ✅ **Combined feature vector** creation from all channels
- ✅ Clean **visualizations** (blobs overlaid on grayscale slice)

---

##  Why This Matters

This prototype demonstrates the viability of:
- Detecting candidates from **N-channel input**
- Creating a **combined feature representation**
- Preparing input for a future **multi-class classifier**

It aligns directly with **Week 1–2 deliverables** from my [GSoC 2025 proposal](https://drive.google.com/file/d/1H7DuvaXul9I2jDgQjpWhkmfbRYuMmFH4/view?usp=sharing).

---

##  Feedback Welcome!

I’m actively working on this as part of my GSoC preparation.  
Feel free to open issues, suggestions, or reach out via Zulip!

---

##  Built With

- Python 
- NumPy
- Matplotlib
- scikit-image
- Synthetic 3D brain data

---

##  Related Links

- 📄 [Cellfinder Paper](https://doi.org/10.1371/journal.pcbi.1009074)
- 🧠 [BrainGlobe Tools](https://brainglobe.info/)
- 🌱 [My GSoC Proposal](https://drive.google.com/file/d/1H7DuvaXul9I2jDgQjpWhkmfbRYuMmFH4/view?usp=sharing)

---

##  Author

**Prisha Sharma**  
GSoC 2025 Applicant | Open-source Contributor | Scientific ML Enthusiast  
[LinkedIn]([https://www.linkedin.com/in/prisha-sharma-788269258/]) · [GitHub](https://github.com/parharti)
