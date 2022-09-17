# JVZY
## Joint-Vertic ZhuYin dataset for object detection and image inpainting

### 建立注音符號專用的深度模型訓練集，可供物件偵測模型對注音符號進行位置偵測，將取得之注音符號邊界框用於影像復原技術，即可將注音符號之區域抹除。

Optical Character Recognition (OCR) [3] technology has also been greatly improved, so the digitization of document has reached the highest efficiency. However, since the texts of this period will have Mandarin Phonetic Symbols (aka Bopomofo and Zhuyin) annotated to facilitate pronunciation learning, the original OCR efficiency will be affected when these phonetic characters are digitized. So,  the essential premise is that there needs to be an appropriate number of phonetic symbol datasets for retraining the OCR model and training a phonetic symbols detector for image inpainting.

全球至少有22億人面臨視覺障礙的問題(WHO 2019)，因人口老齡化與生活方式的改變，也致使視障人數逐年增加。而台灣則有約4萬6千名視障人口(伊甸社會福利基金會)。本計畫將學童之課內、外讀物轉換成文字讀本時，能減少OCR對注音文本的辨識錯誤率，因此減少後續人工逐字檢查、重新繕打的工作量，提高自動導讀、有聲書與電子書的製作效率。使視障孩子能夠閱讀與同齡孩子相同的書籍資源，進而阻絕視障生的學習弱勢，協助導向正常社交和人際關係。
現行讀物轉換成文字讀的方法，係掃描讀本後存為數位影像，再利用商用OCR軟體辨識後輸出文字檔。本團隊提供注音抹除工具能夠將掃描後的數位影像中的注音符號消除，並保留其他原有畫面，再由慣行的OCR軟體辨識。因此我們所規劃的方法是可以直接加入現行工作流程，而不需要進行太多的系統修改，也不影響現行方式的習慣性。

國小1-4年級的學生正值語言學習的黃金期，閱讀能力需要大量透過圖文書和繪本輔助進行培養，目前讀物和教材皆有大量旁註注音以協助一般明眼學生來閱讀，然而對視障學生來說，相同的圖文書籍只能仰賴家長的報讀外，主要是利用文字辨識技術(OCR)先將書籍文字轉換成純文字檔，後續再重製為點字書與有聲書。但現行Optical Character Recognition (OCR) 技術對於有旁註注音的中文字容易產生辨識錯誤或是辨識成亂碼（如下圖），也不利於直接使用OCR軟體進行導讀。導致對於有注音的文本不論是在純文字的辨識重製上，以及後續人工校對的耗時費力上造成更重的負擔。

#### 旁註注音對OCR的影響
![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_1_issue.jpg)
![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_2_issue.jpg)

#### 量化旁註注音對OCR的影響
##### (w：有旁註注音在Recall, F-score指標均大幅降低。)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/fig6.jpg)

#### 注音訓練集與注音偵測模型 
![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_3_workflow.jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/v1_4_zy_detection.jpg)
  
  
  
---------------------------------------


---------------------------------------

# JVZYv2
## Joint-Variant ZhuYin dataset for Image-to-Image training

#### 建立注音符號專用的深度模型訓練集，可供Image-to-Image模型的訓練，可將輸入影像中的注音符號過濾去除。

#### 在影像解析度為640x640下之抹除樣本(左：輸入原始旁註注音影像，中：模型輸出無注音影像，右：無旁註之ground truth影像。)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[0].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[10].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[1].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[3].jpg)

![Image text](https://github.com/vscv/JVZY/blob/main/samples/zhuyin_result_evl[7].jpg)

##### NOTE: This is JVZY v2 dataset only for image2image networks.

---------------------------------------


If you find this code useful in your research, please consider citing:

@inproceedings{ss,
Author = {ssss},
Title = {Cssss},
Booktitle  = {sssssss},
Year = {2023}
}

---------------------------------------
