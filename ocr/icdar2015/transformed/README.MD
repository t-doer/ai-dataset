# Transform Data

## 1. Unzip and Organize File Structure

```
train_data
  |--detection
       |--test
            |--gt (<= Challenge4_Test_Task1_GT.zip)
                |--gt_img_1.txt
                |--gt_img_2.txt
                |-- ...
                |--gt_img_500.txt
            |--imgs (<= ch4_test_images.zip)
                |--img_1.jpg
                |--img_2.jpg
                |-- ...
                |--img_500.jpg
       |--train
            |--gt (<= ch4_training_localization_transcription_gt.zip)
                |--gt_img_1.txt
                |--gt_img_2.txt
                |-- ...
                |--gt_img_1000.txt
            |--imgs (<= ch4_training_images.zip)
                |--img_1.jpg
                |--img_2.jpg
                |-- ...
                |--img_1000.jpg
  |--recognition
       |--test (<= ch4_test_word_images_gt.zip)
            |--gt.txt (<= Challenge4_Test_Task3_GT.txt)
            |--coords.txt
            |--word_1.png
            |--word_2.png
            |--...
            |--word_2077.png 

       |--train (<= ch4_training_word_images_gt.zip)
            |--gt.txt
            |--coords.txt
            |--word_1.png
            |--word_2.png
            |--...
            |--word_4468.png           
```

## 2. Commands

```shell script
mkdir -p train_data/detection/{test,train}/{gt,imgs}
mkdir -p train_data/recognition/{test,train}
unzip Challenge4_Test_Task1_GT.zip -d train_data/detection/test/gt
unzip ch4_test_images.zip -d train_data/detection/test/imgs
unzip ch4_training_localization_transcription_gt.zip -d train_data/detection/train/gt
unzip ch4_training_images.zip -d train_data/detection/train/imgs
unzip ch4_test_word_images_gt.zip -d train_data/recognition/test/
unzip ch4_training_word_images_gt.zip -d train_data/recognition/train/
mv Challenge4_Test_Task3_GT.txt train_data/recognition/test/gt.txt
```