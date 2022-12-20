# ASM-Block-iRule

Block illegal client ip if it violate ASM policy in a specific rate:


set static::maxRate 50 ----- Number of violations


set static::windowSecs 300 ----- Duration of violations in seconds


set static::holdtime 600 ----- Block duration in seconds
