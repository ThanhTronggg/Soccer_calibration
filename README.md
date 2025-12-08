# Soccer Calibration - Data Location Guide

## Tổng quan
Project này bao gồm 3 notebook chính để xử lý và phân tích dữ liệu bóng đá:
- **Map_2d.ipynb**: Mapping 2D sân bóng
- **model-detect-keypoint.ipynb**: Phát hiện keypoint trên sân
- **model-detect-player.ipynb**: Phát hiện cầu thủ

## Vị trí dữ liệu (Data Location)

### 1. model-detect-keypoint.ipynb
**Dataset được sử dụng**: Football Field Detection (Keypoints)

**Roboflow Project**:
- Workspace: `iot-ch2d2`
- Project: `football-field-detection-f07vi-8n9pw`
- Version: 5
- Format: YOLOv8
- Link: https://universe.roboflow.com/iot-ch2d2/football-field-detection-f07vi-8n9pw/5

**Số lượng dữ liệu**:
- Training images: 855 ảnh
- Test images: 32 ảnh
- Valid images: 40 ảnh

**Keypoints**: 32 điểm đặc trưng trên sân bóng (góc sân, vạch vôi, v.v.)

---

### 2. model-detect-player.ipynb
**Dataset được sử dụng**: Football Players Detection

**Roboflow Project**:
- Workspace: `roboflow-jvuqo`
- Project: `football-players-detection-3zvbc`
- Version: 12
- Format: YOLOv8
- Link: https://universe.roboflow.com/roboflow-jvuqo/football-players-detection-3zvbc/12

**Số lượng dữ liệu**:
- Training images: 298 ảnh
- Test images: 25 ảnh
- Valid images: 49 ảnh

**Classes**: 4 lớp đối tượng
1. `ball` - Bóng
2. `goalkeeper` - Thủ môn
3. `player` - Cầu thủ
4. `referee` - Trọng tài

---