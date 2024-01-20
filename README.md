1. mkdir -p DATA/wavs

2. Copy all wavs data from datasets into DATA/wavs

3. Create DATA/train.txt and DATA/test.txt with format:
<WAV_FILE_NAME> <RAW_TEXT>

4. python Step1_data_processing.py

5. python Step2_extract_feature.py

6. cd vits
python train_ms.py -c configs/train.json

or download pretrained model: https://drive.google.com/file/d/1_4IAWOJlEl0oD54KVloEmPGR30Ox2GRx/view?usp=sharing
store in folder: ./VITS_Vietnamese/pretrained/Generator.pth

7. python inference.py
