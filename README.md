# KV-NC20L_Serial_test

## 第一步 : 將USB to Serial 模組中的腳位與KV-NC20L的RS232做連結。

    Serial  -->>    KV-NC20L
    Rx      -->>    SD(A)
    --              SD(B)
    --              RD(A)
    Tx      -->>    RD(B)
    GND     -->>    SG


## 第二步 : 開啟Realterm 做設定

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/1.PNG)

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/2.PNG)

確認連結的PORT是否正確。


## 第三步 : 使用KV STUDIO 開啟 RS232_button.kpr    
    
    按下單元編輯器，如下圖，做設定。

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/KV.PNG)

    按下R000 透過Serial output value。

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/3.PNG)

    便會如圖輸出值。


### 階梯圖備註
    如下圖，使當按鈕按下去後為1，在按一次便為0，達到Switch之效用。

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/T1.PNG)

    如下圖，CM7515設0001的話，資料儲存將為字位元。
    CM7516為預設，剩下標頭與定界符不做設定。

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/T2.PNG)

    如下圖，CM7001設定CM7001的資料長度為3個
    並在後續CM7002 ~ CM7004 給值。

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/T3.PNG)

    如下圖，當按鈕再次按下會關閉。

![image](https://github.com/Uniboy-ROS/KV-NC20L_Serial_test/blob/master/image/T4.PNG)
    



