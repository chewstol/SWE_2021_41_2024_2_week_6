# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
>https://github.com/chewstol/SWE_2021_41_2024_2_week_4
<pre>
  <code>
    def isHappy(n):

  count = 0
  num = n
  buf = 0
  loops = [-1]

  while num not in loops:
    loops += [num]
    buf = 0
    while num != 0:
      buf += (num%10)*(num%10)
      num = num//10
    if buf == 1:
      return True
    if buf in loops:
      return False
    if buf not in loops:
      num = buf
      print(loops)

  return False

  </code>
</pre>
