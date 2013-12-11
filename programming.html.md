title: 令人汗顏的programming能力…
date: 2004-09-09 22:57:00
tags: 
- development
---

這幾天我嘗試解一個大專軟體設計比賽的題目，是2002年的第一題。
作了之後才知道，我的programming能力實在是不夠強。我看還有得磨的呢....
我解了一半，還有些問題待解決，Post題目跟我的想法給大家笑笑 :D

[題目](http://wshlab2.ee.kuas.edu.tw/~yurenju/files/PA.pdf), [輸入檔](http://wshlab2.ee.kuas.edu.tw/~yurenju/files/pa.txt)

大意是這樣的：有個人種了幾棵樹，然後現在他想沿著最外面的樹建立圍牆，請問這個把樹都圍起來的牆最短的長度是多少？
<a name='more'></a>
以一個門外漢的思考角度(我還沒學過演算法)，我是這麼想的：
* 先把樹的座標從檔案裡面讀出來，放在link list以供調用
* 找出x min, x  max, y min, y max的樹的座標，放入另一link list中。
* 用 x min與y min的樹座標算出直線公式，比較其他樹座標是在這直線的上方或是下方
* 另外的條件：被比較的樹座標其x軸座標必須在上面提的那兩點座標之間。
* 如果在下方，則把他插入list當中。
* 然後在從頭搜尋
* 依此類推....

不過這樣作有個缺點，就是他只能找出樹的邊緣，但是卻不能找出最短距離。

後來想想，這應該有什麼特別的方法可以解，用土法煉鋼的方法，可是會讓人笑掉大牙的 XD