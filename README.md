
![image](https://user-images.githubusercontent.com/120350543/217751673-01c34d69-f447-436a-9722-93d185eba1ab.png)

备注：

Block illegal client ip if it violate ASM policy in a specific rate:


set static::maxRate 50 ----- Number of violations


set static::windowSecs 300 ----- Duration of violations in seconds


set static::holdtime 600 ----- Block duration in seconds
