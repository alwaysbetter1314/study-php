# study-php
learning php
## 数组使用
```
<?php 
// 索引数组。
$arr = array('fuck','shit','hh');
forEach($arr as $i){
    echo $i."\n";
}
// key-value数组
$kvarr = array('hello'=>'world','fuck'=>'shit');
echo $kvarr['hello'],"\n";
foreach($kvarr as $i=>$i_value) {
  echo "Key=" . $i . ", Value=" . $i_value;
  echo "<br>";
}
// 二维数组
$tdimarr = array(
    array('fuck','shit','damn'),
    array('it','she','he'),
    array('we','i','ri')
);
forEach($tdimarr as $i){
    forEach($i as $j){
        echo $j.'-';
    }
    echo "\n"; 
}
//数组追加元素
array_push($arr,'cao','wdnmd');
echo current($arr);
// 数组合并数组
//  ① next：将数组指针，后移一位。并返回后一位的值；没有返回false
//    ② prev：将数组指针，前移一位。并返回前一位的值；没有返回false
//    ③ end：  将数组指针，移至最后一位，返回最后一位的值；空数组返回false
//    ④ reset:将数组指针，恢复到第一位。并返回第一位的值；空数组返回false
//    ⑤ key: 返回当前指针所在位的键；
//    ⑥ current:返回当前指针所在位的值；
$newarr = array_merge($arr,array('11','22'));
echo end($newarr);
// array_merge_recursive() 同上，已有key的键值会合并。
//array_combine() 两个等长索引数组形成一个kv数组。

```
