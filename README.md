# JVZY
## Joint-Vertic ZhuYin dataset for object detection and image inpainting

### 建立注音符號專用的深度模型訓練集，可供物件偵測模型對注音符號進行位置偵測，將取得之注音符號邊界框用於影像復原技術，即可將注音符號之區域抹除。

Optical Character Recognition (OCR) [3] technology has also been greatly improved, so the digitization of document has reached the highest efficiency. However, since the texts of this period will have Mandarin Phonetic Symbols (aka Bopomofo and Zhuyin) annotated to facilitate pronunciation learning, the original OCR efficiency will be affected when these phonetic characters are digitized. So,  the essential premise is that there needs to be an appropriate number of phonetic symbol datasets for retraining the OCR model and training a phonetic symbols detector for image inpainting.


#### 旁註注音對OCR的影響
![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_1_issue.jpg)
![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_2_issue.jpg)

#### 注音訓練集與注音偵測模型
![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_3_workflow.jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_4_zy_detection.jpg)
  
  
  
---------------------------------------


---------------------------------------

# JVZYv2
## Joint-Variant ZhuYin dataset for Image-to-Image training

#### 建立注音符號專用的深度模型訓練集，可供Image-to-Image模型的訓練，可將輸入影像中的注音符號直接抹除。

#### 在影像解析度為640x640下之抹除樣本(左：輸入原始旁註注音影像，中：模型輸出無注音影像，右：無旁註之ground truth影像。)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[0].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[10].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[1].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[3].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[7].jpg)

---------------------------------------
