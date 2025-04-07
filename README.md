
# Brain tumor detection

With the use of CNN algo and pre-trained model (yolov11n), i fine-tuned the model to detect tumors smartly.




## Run Locally

Clone the project

```bash
  git clone https://github.com/marcusxro/brain-tumor-ai-detector
```

Go to the project directory

```bash
  cd cd brain-tumor-ai-detector
```

Set Up a Virtual Environment (Optional, but Recommended)

```bash
  python -m venv myenv
```

Activate the venv

```bash
 myenv\Scripts\activate
```

Install Dependencies

```bash
 pip install -r requirements.txt
```

To Train the Model:

```bash
!yolo detect train data=/content/data.yaml model=yolo11s.pt epochs=60 imgsz=640
```


Test the model:

```
!yolo detect predict model=runs/detect/train/weights/best.pt source=data/validation/images save=True
```
## Screenshots
![App Screenshot](https://raw.githubusercontent.com/marcusxro/brain-tumor-ai-detector/refs/heads/main/result2-ezgif.com-video-to-gif-converter.gif)

![App Screenshot](https://raw.githubusercontent.com/marcusxro/brain-tumor-ai-detector/refs/heads/main/train/train_batch0.jpg)



![App Screenshot](https://raw.githubusercontent.com/marcusxro/brain-tumor-ai-detector/refs/heads/main/train/train_batch901.jpg)

## Badges

Add badges from somewhere like: [shields.io](https://shields.io/)

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/)
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)


## Authors

- [@marcusxro](https://www.github.com/marcusxro)

