# robosys2020_lesson7
ロボットシステム学の講義第7、8回で作成したデバイスドライバです。
講義のコードに2を与えたらLEDが点滅するプログラムを加えました。


デバイスドライバ　https://github.com/kaba92/robosys2020_lesson7/blob/main/myled.c

Makefile https://github.com/kaba92/robosys2020_lesson7/blob/main/Makefile


使用したOS

・Ubuntu 18.04



使用した道具

・Raspberry　Pi4

・LED　1個

・220Ω抵抗　1個

・F-Mジャンパー線　2個

・ブレッドボード


以下のコマンドを順に入力するとLEDを点滅する。

make

sudo rmmod myled

sudo insmod myled.ko

chmod 666 /dev/myled0

echo 2 > /dev/myled0　 //LEDを点滅させる


ライセンス　https://github.com/kaba92/robosys2020_lesson7/blob/main/LICENSE


実行したときの動画　http://www.youtube.com/watch?v=_6X7jtEPQpU
