Poetry Generator with Text Image

Team members: Sophia Song(xsong2), Yuming Fu(yfu49), Yongxuan Fu(yfu13)

Team Name: The Powerpuff Girls

Getting Started

Download Glove for poem generate model:
1. Download glove.6B.200d.txt from https://drive.google.com/file/d/1ZNNQuy-dBQ7sLfAOs198dcnBq55CPQtv/view
2. Add glove file into data/

Download pretrained model for deep text recognition bench model
1. Download pretrained model - TRBA (TPS-ResNet-BiLSTM-Attn) - from https://drive.google.com/drive/folders/15WPsuPJDCzhp2SvYZLRj8mAlT3zmoAMW
2. Add image files to test into demo_image/
3. Run demo.py (add --sensitive option if you use case-sensitive model)

python3 demo.py \
--Transformation TPS --FeatureExtraction ResNet --SequenceModeling BiLSTM --Prediction Attn \
--image_folder demo_image/ \
--saved_model TPS-ResNet-BiLSTM-Attn.pth
