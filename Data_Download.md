📦 Downloading the Wound Healing Dataset
This repository contains code for wound healing analysis. The full image dataset is managed separately due to its size (~800 MB).

    Important: You must have Git LFS (Large File Storage) installed to download the actual images. Without it, you will only get small text pointers that reference the large files (not the files themselves). Install Git LFS from git-lfs.com and initialize it on your system with git lfs install after installation.

Option 1: Clone the Full Project (Recommended)
This method will download both the project code (scripts, documentation, configuration) and the complete wound healing dataset (via Git LFS). It is the best choice for most users who want to run the analysis code or work with the full project.
Step-by-Step Instructions
bash
运行

# 1. Clone the remote repository to your local machine
# This downloads regular project files and Git LFS pointer files (not the actual large images yet)
git clone https://github.com/hjconde/WoundHealingDetection.git

# 2. Navigate into the root directory of the cloned project
# (Mandatory: Git LFS commands must be run within the project repository directory)
cd WoundHealingDetection

# 3. Fetch the actual large image files from the Git LFS server
# This converts the LFS pointer files into the real ~800 MB image dataset
git lfs pull

Option 2: Download Only the Dataset (For Existing Local Repositories)
This method is intended for users who have already cloned the WoundHealingDetection repository locally (and only need to fetch the image dataset, or want to avoid downloading unnecessary files). It allows you to pull only the wound_healing_data/ directory (containing the raw images) without re-cloning the entire project.
Step-by-Step Instructions

    Ensure you have Git LFS installed and configured on your system (run git lfs install if you haven't already).
    Navigate into the root directory of your existing local WoundHealingDetection repository:
    bash

运行

cd WoundHealingDetection

Run the following command to pull only the large files in the wound_healing_data/ directory:
bash
运行

git lfs pull --include="wound_healing_data/"
