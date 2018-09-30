# python-creation-of-virtual-environments

如何使用 venv 建立 virtual environments  📝

* [Youtube Tutorial - How to use venv to create virtual environments - python](https://youtu.be/LzaBf2QjR8s)


## 簡介

在 python 中，我們常常需要建立環境應付各個 project，如果沒有切割環境，會非常難維護，

所以，建立 virtual environments 是一件非常重要的事情:satisfied:

以前我也有介紹過如何建立 virtual environments，那時候是使用 Anaconda，文章可參考 [這裡](https://github.com/twtrubiks/FaceDetect/tree/master/How%20Easy%20Install%20OpenCV%20%20for%20Python%20use%20Anaconda)，

不過最近重灌電腦，就覺得裝 Anaconda 超級花時間( 因為 Anaconda 檔案略大:persevere: )，

而且正式機上，通常也不太會使用 Anaconda 建立環境，所以，今天就和大家介紹官方文件建議的做法，

使用 [venv](https://docs.python.org/3/library/venv.html) 建立 virtual environments 吧:grinning:

## 教學

### 安裝 python
首先，一定要先下載 [python](https://www.python.org/downloads/)，當你在安裝時，他會問你是否要加入環境變數，請記得要把他打勾:thumbsup:

預設是沒有打勾的，安裝完畢後，使用 terminal 輸入 python ( 或 python3 ) 確認是否可以找到 ( 如下圖 )，

![alt tag](https://i.imgur.com/sL7tfoF.png)

如果出現 `'python' 不是內部或外部命令、可執行的程式或批次檔。`，就代表你的環境變數沒設定。

( 有兩種方法可以解決，第一種是移除 python 重新安裝，然後安裝時記得打勾加入環境變數， 第二種是自己加入環境變數 )

，環境變數的部分如下，像是我自己有裝兩種不同版本的 python，

![alt tag](https://i.imgur.com/RDhWhoO.png)

### 如何使用 venv 建立 virtual environments

首先，切到目錄 (看你想要統一 venv 在哪個資料夾)底下，接著執行以下指令，

```cmd
python -m venv tutorial-venv
```

![alt tag](https://i.imgur.com/hG1vSoh.png)

如上圖，當右邊的指令執行完之後，目標資料夾底下就會多出一個 tutorial-venv ( 你所指定的名稱 )。

### 如何啟動 virtual environments

要啟動 virtual environments 也很簡單，直接執行 activate.bat，他在 tutorial-venv/Scripts/activate.bat 底下，

```cmd
tutorial-venv\Scripts\activate.bat
```

如下圖，執行在 terminal 中輸入 `activate.bat` 即可，

![alt tag](https://i.imgur.com/zTrvEP8.png)

如上圖，這樣就成功啟動 virtual environments 了:satisfied:

如果想要關閉或退出，執行 deactivate.bat 即可，如下圖，

![alt tag](https://i.imgur.com/R8Y9fma.png)

在該環境下安裝的任何 library 都不會去影響到其他的 virtual environments，

舉個例子，如下圖，我在 tutorial-venv 環境中安裝了 requests，所安裝的 library，

是不會去影響到其他的 virtual environments，

( 下圖左邊為本機的 python，下圖右邊為 virtual environments )

![alt tag](https://i.imgur.com/NicARVa.png)

可以看到，在 virtual environments 中安裝的 requests 是不會影響到本機中的 python 環境:thumbsup:

最後，依照自己使用的 ide 把 venv 環境指定好就可以了:relaxed:

## 執行環境

* windows 10

## Reference

* [Creation of virtual environments](https://docs.python.org/3/library/venv.html)

## Donation

文章都是我自己研究內化後原創，如果有幫助到您，也想鼓勵我的話，歡迎請我喝一杯咖啡:laughing:

![alt tag](https://i.imgur.com/LRct9xa.png)

[贊助者付款](https://payment.opay.tw/Broadcaster/Donate/9E47FDEF85ABE383A0F5FC6A218606F8)

## License

MIT license
