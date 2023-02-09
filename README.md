背景：
传统的AWAF防护方式只能选择固定的放行或者阻断，无法定义周期性的策略
默认的阻拦策略无法进行多维度综合分析，例如基于多种违规类型阻断或多种违规等级并结合攻击频次设置阻断策略

使用场景：
在应用服务器前端，通过iRules智能识别非法用户的攻击类型或请求违规等级，直接阻断非法客户端的IP。

解决方案：
用户自定义违规等级，攻击检测频次和阻断时间等参数。
iRules自动识别攻击命中频次，超出阈值即将攻击客户端IP拉黑并阻断指定的时间

客户收益：
更加灵活，安全的攻击防御手段，有效降低误报。
自动化的IP Block策略，无需维护，降低设备性能消耗。

核心业务：
门户应用，交易应用
HTTP/HTTPS

![image](https://user-images.githubusercontent.com/120350543/217751673-01c34d69-f447-436a-9722-93d185eba1ab.png)

备注：
# ASM-Block-iRule

Block illegal client ip if it violate ASM policy in a specific rate:


set static::maxRate 50 ----- Number of violations


set static::windowSecs 300 ----- Duration of violations in seconds


set static::holdtime 600 ----- Block duration in seconds
