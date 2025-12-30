## 📦 Downloading the Wound Healing Dataset

This repository contains code for wound healing analysis. The full image dataset is managed separately due to its size (~800 MB).

> **Important**: You must have **Git LFS (Large File Storage)** installed to download the actual images. Without it, you will only get small text pointers. Install it from [git-lfs.com](https://git-lfs.com).

### Option 1: Clone the Full Project (Recommended)

This will download both the code and the dataset.

```bash
# 1. Clone the repository (this downloads the code and LFS file pointers)
git clone https://github.com/hjconde/WoundHealingDetection.git

# 2. Navigate into the project directory
cd WoundHealingDetection

# 3. Fetch the actual large image files from Git LFS
git lfs pull

Option 2: Download Only the Dataset

If you are only interested in the raw images, you can download the complete wound_healing_data folder directly:

    Ensure you have Git LFS installed and configured on your system.

    Run the following command to pull only the data directory:
    bash

git lfs pull --include="wound_healing_data/"

Alternatively, you can browse and download individual files via the GitHub webpage, but you must ensure your Git LFS client is active to convert pointers into real files.
