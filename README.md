C言語

問題1.動的ローカル変数宣言後にEclipseでgdbモードでデフォルト値0になっている
 【持っている知識】
  ◇未初期化
   不定値なのに

 【調査結果】
  動的変数はメモリスタック領域を利用するため、初期化の時点でスタックメモリに格納されている値が初期値となる。
  未初期化のメモリには 0 が格納されていることが多いが、必ずしもそうとは限らない。
  
  【質問】
   なぜwhy 未初期化のメモリには 0 が格納されていることが多い？
   もし、分かっている人はいるなら、ご教示お願い致します。