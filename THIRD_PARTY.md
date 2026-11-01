# Сторонние библиотеки, модели и данные

Лицензия MIT в этом репозитории относится только к коду проекта. Сторонние компоненты сохраняют свои лицензии.
Веса итогового решения не распространяются: они обучены на данных постановщика, а часть из них дополнительно связана
некоммерческими условиями, указанными ниже.

## Модели и данные

| Компонент | Лицензия | Как использован |
|---|---|---|
| object-CXR (JF Healthcare, MIDL 2020) | CC BY-NC 4.0, некоммерческое использование | предобучение сетей по посторонним предметам и карты предметов; данные в репозиторий не входят |
| FleXray (Butoi V. et al., MIT CSAIL), веса `VictorButoi/flexray` | CC BY-NC 4.0, некоммерческое использование; пакет `flexray` под MIT | необязательный модуль сегментации; веса в репозиторий не входят, без них модуль выключен |
| TorchXRayVision, веса `densenet121-res224-all` (Cohen JP et al.) | основная библиотека Apache-2.0, условия подмоделей различаются | начальные веса DenseNet121 при обучении |
| ResNet18, EfficientNet-B0, DenseNet121 из torchvision | код BSD-3-Clause, веса обучены на ImageNet | начальные веса |
| DINOv2 | Apache-2.0 | только опыт, в решение не вошла |
| RadImageNet, RAD-DINO | условия авторов моделей | только опыт, веса в репозиторий не входят |

При коммерческом внедрении модуль FleXray нужно отключить, а сети, предобученные на object-CXR, заменить.

## Библиотеки

| Компонент | Лицензия |
|---|---|
| PyTorch, torchvision | BSD-3-Clause |
| timm | Apache-2.0 |
| OpenCV | Apache-2.0 |
| NumPy, pandas, scikit-learn, scikit-image | BSD-3-Clause |
| pydicom, pylibjpeg, pylibjpeg-openjpeg | MIT |
| python-gdcm | Apache-2.0 |
| FastAPI | MIT |
| uvicorn | BSD-3-Clause |
| openpyxl | MIT |
| Pillow | MIT-CMU |
| pytest | MIT |
| Шрифты DejaVu (`src/dxaqc/fonts/`) | свободная лицензия, текст в `LICENSE_DEJAVU.txt` |
