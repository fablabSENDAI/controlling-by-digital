---
layout: default
title: スイッチでの入力
parent: Arduino
nav_order: 2
---

# **スイッチでの入力**

### 配線
<img src="assets/arduino_io.png"  alt="hi" class="inline"/>


### コード

```c++
void setup()
{
  pinMode(7, INPUT);
  pinMode(13, OUTPUT);
}

void loop()
{
  if(digitalRead(7)){
    digitalWrite(13,LOW);
  }else{
    digitalWrite(13,HIGH);
  }
}
```
