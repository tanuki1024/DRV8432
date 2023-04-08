# DRV8432
12V：12Vには必ず10.8~13.2の間で入れてください

GND：GNDをつないでください。

OUT1+,OUT1-：１個目のモーターをここにつないでください。

OUT2+,OUT2-：２個目のモーターをここにつないでください。

PWM1：１個目のモーターを操作するピンです。ここにPWMをぶち込んでください。
これはPWMのduty比(ONとOFFの比)を0%とか100%とかで入れると変な挙動をするので
だいたいduty比が3~97%の割合で値を入れてください。
ちょうどduty比が50%で停止します。
動作電圧は3.3vなのでArduinoで使いたい人はロジック変換を乗せてください。

PWM2：２個目のモーターを操作するピンです。

RESET：ここは通常は触らなくていいですが、
モーターのブレーキ停止がしたくない場合はここをLOWにしてください。
あとこうすると停止してる時に電流が流れなくなるので節電できます。
LAP駆動は電流バカ食うのでついてあるといいです。
これは普通はHIGHに設定されています。
動作電圧は3.3vなのでArduinoで使いたい人はロジック変換を乗せてください。
