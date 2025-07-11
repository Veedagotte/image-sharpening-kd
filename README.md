# image-sharpening-kd
“Image sharpening using knowledge distillation for real-time video conferencing.”
# Image Sharpening using Knowledge Distillation

This project implements a student-teacher knowledge distillation framework to enhance image sharpness for video conferencing under low-bandwidth conditions.

## 🧠 Model Summary

- **Teacher Model**: High-quality image as ground truth.
- **Student Model**: Lightweight CNN trained to mimic the teacher output.
- **Loss Function**: MSE
- **Metric**: SSIM (target > 0.9)

## 📁 Files

- `image_sharpening_kd.ipynb`: Full training pipeline in Google Colab.
- `report_summary.txt` or `report.pdf`: Contains problem definition, approach, evaluation.

## 📊 Output

- Average SSIM: ~0.91+
- FPS Target: 30-60fps on optimized student model

## 📷 Dataset

Sample dataset created by downscaling and upscaling uploaded high-res images using bicubic interpolation.

---

## ✅ How to Run

1. Open `image_sharpening_kd.ipynb` in Google Colab
2. Upload your high-res image samples
3. Run all cells
4. Observe model training and SSIM output
