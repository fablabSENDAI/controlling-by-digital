---
layout: default
title: モーターの逆転
parent: Arduino
nav_order: 3
---

# **モーターの逆転**

### 配線

<img src="assets/motor_reverse.png"  alt="hi" class="inline"/>

### コード

```c++
void setup()
{
  pinMode(7, OUTPUT);
  pinMode(8, OUTPUT);
}

void loop()
{
  //seiten
  digitalWrite(7, HIGH);
  digitalWrite(8, LOW);
  delay(3000); // Wait for 3000 millisecond(s)

  //break
  digitalWrite(7, LOW);
  digitalWrite(8, LOW);
  delay(100); // Wait for 100 millisecond(s)

  //gyakauten
  digitalWrite(7, LOW);
  digitalWrite(8, HIGH);
  delay(3000); // Wait for 3000 millisecond(s)

  //break
  digitalWrite(7, LOW);
  digitalWrite(8, LOW);
  delay(100); // Wait for 100 millisecond(s)
}
```
