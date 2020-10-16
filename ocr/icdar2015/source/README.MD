# ICDAR2015

Downloaded from https://rrc.cvc.uab.es/?ch=4&com=downloads, on October 2020.

## Text Localization

`ch4_training_images.zip` - Text Localization / Training Set - Images

Training Set Images (88.5MB).- 1000 images obtained with wearable cameras

- File Structure
    
    ```
    img_1.jpg
    img_2.jpg
    ...
    img_1000.jpg
    ```
    
`ch4_training_localization_transcription_gt.zip` - Text Localization / Training Set - Transcription

Training Set Localisation and Transcription Ground Truth (157KB).- 1000 text files with word level localisation and transcription ground truth

- File Structure
    
    ```
    gt_img_1.txt
    gt_img_2.txt
    ...
    gt_img_1000.txt
    ```
    
- Data Structure

    For example, `gt_img_1.txt`:
    
    ```
    377,117,463,117,465,130,378,130,Genaxis Theatre
    493,115,519,115,519,131,493,131,[06]
    374,155,409,155,409,170,374,170,###
    492,151,551,151,551,170,492,170,62-03
    376,198,422,198,422,212,376,212,Carpark
    494,190,539,189,539,205,494,206,###
    374,1,494,0,492,85,372,86,###

    ```

`ch4_test_images.zip` - Text Localization / Test Set - Images

Test Set Images (43.3MB).- 500 images obtained with wearable cameras. You can submit your results for this Task over the images of the test set through the My Methods section.

- File Structure
    
    ```
    img_1.jpg
    img_2.jpg
    ...
    img_500.jpg
    ```
    
`Challenge4_Test_Task1_GT.zip` - Text Localization / Test Set -  text localisation bounding boxes

Test Set Ground Truth (244Kb). - 500 text files with text localisation bounding boxes for the images of the test set.

- File Structure
    
    ```
    gt_img_1.txt
    gt_img_2.txt
    ...
    gt_img_500.txt
    ```
    
- Data Structure

    For example, `gt_img_1.txt`:
    
    ```
    933,255,954,255,956,277,936,277,###
    172,323,195,324,195,339,177,339,###
    83,270,118,271,115,294,88,291,###
    940,310,962,310,962,320,940,320,###
    946,356,976,351,978,368,950,374,###
    940,322,962,322,964,333,943,334,###
    128,344,210,342,206,361,128,362,###
    312,303,360,303,360,312,312,312,###

    ```
    
## Word Recognition

`ch4_training_word_images_gt.zip` - Word Recognition / Training Set - Images and Transcriptions

Training Set Word Images, along with Transcriptions Ground truth (40.5MB).- ~4468 cut out word images corresponding to the axis oriented bounding boxes of the words are provided along with a single text file with the relative coordinates of the bounding shape within each word image. Transcription ground truth is provided in a single txt file.

- File Structure
    
    ```
    gt.txt       - Ã¿ÕÅÍ¼Æ¬¶ÔÓ¦µÄÎÄ×Ö
    coords.txt   - Ã¿ÕÅÍ¼Æ¬¶ÔÓ¦µÄ×ø±êÏµ
    word_1.png
    word_2.png
    ...
    word_4468.png
    ```

- Data Structure
    
    - gt.txt
        
        ```
        word_1.png, "Genaxis Theatre"
        word_2.png, "[06]"
        word_3.png, "62-03"
        word_4.png, "Carpark"
        word_5.png, "EXIT"
        word_6.png, "I2R"
        word_7.png, "fusionopolis"
        word_8.png, "fusionopolis"
        ```
        
    - coords.txt
        
        ```
        word_1.png,0,0,86,0,88,13,1,13
        word_2.png,0,0,26,0,26,16,0,16
        word_3.png,0,0,59,0,59,19,0,19
        word_4.png,0,0,46,0,46,14,0,14
        word_5.png,0,0,33,2,32,24,0,23
        word_6.png,0,0,58,10,58,54,4,51
        word_7.png,0,9,133,0,136,43,3,52
        word_8.png,0,0,90,8,91,45,1,46
        ```
    
`ch4_test_word_images_gt.zip` - Word Recognition / Test Set - Images

Test Set Word Images (21.5MB).- 2077 cut out word images corresponding to the axis oriented bounding boxes of the words are provided along with a single text file with the relative coordinates of the bounding shape within each word image. You can submit your results for this Task over the images of the test set through the My Methods section.

- File Structure
    
    ```
    coords.txt   - Ã¿ÕÅÍ¼Æ¬¶ÔÓ¦µÄ×ø±êÏµ
    word_1.png
    word_2.png
    ...
    word_2077.png
    ```

- Data Structure

    - coords.txt
        
        ```
        word_1.png,0,0,113,2,112,33,0,33
        word_2.png,0,2,50,0,49,12,1,14
        word_3.png,0,0,24,1,24,15,0,14
        word_4.png,0,0,23,1,23,14,1,13
        word_5.png,0,0,25,1,25,13,0,13
        word_6.png,0,0,25,1,26,14,0,13
        word_7.png,0,0,40,3,40,17,0,14
        word_8.png,0,0,29,0,29,13,0,13
        ```

`Challenge4_Test_Task3_GT.txt` - Word Recognition / Test Set - Transcriptions

Test Set Ground Truth (49Kb). - A single text file with the transcriptions of the 2077 images of the test set. Each line corresponds to an image of the test set.

- Data Structure

    ```
    word_1.png, "JOINT"
    word_2.png, "yourself"
    word_3.png, "154"
    word_4.png, "197"
    word_5.png, "727"
    word_6.png, "198"
    word_7.png, "20029"
    word_8.png, "Free"
    ```
    
## References

- Description: https://rrc.cvc.uab.es/?ch=4
- Other source: https://github.com/WenmuZhou/OCR_DataSet