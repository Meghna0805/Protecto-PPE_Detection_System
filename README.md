# PPE Detection Using YOLO-NAS 

This project implements a Personal Protective Equipment (PPE) detection system using the YOLO-NAS object detection model. It is designed to identify safety gear like helmets, vests, gloves, and masks in images and videos — useful for surveillance in construction sites or factories.

---

##  Features

- Trained YOLO-NAS Small on a custom dataset with 3,235 images and 7 PPE classes.
- Achieved **80.2% mAP@0.5** and **98.28% Recall** on validation data.
- Tested on real CCTV footage for accurate detection of:
  -  Helmets
  -  Gloves
  -  Masks
  -  Safety Jackets
  -  Safety Harness (if available)
- Real-time tracking can be integrated using DeepSORT (optional).

---

##  Model Training Details

- **Model**: YOLO-NAS Small (via SuperGradients)
- **Dataset**: Roboflow-annotated PPE safety dataset
- **Epochs**: 10
- **Batch Size**: 8
- **Input Resolution**: 640 × 640

---

##  Results

| Metric      | Value   |
|-------------|---------|
| mAP@0.5     | 80.2%   |
| Recall      | 98.28%  |
| Precision   | ~85%    |
| FPS (GPU)   | ~45 FPS |

---

##  Dependencies

- `super-gradients`
- `torch`
- `opencv-python`
- `matplotlib`
- `roboflow`

---

##  Future Enhancements

- [ ] Real-time webcam deployment
- [ ] Integration with DeepSORT for object tracking
- [ ] Alert system for missing PPE

