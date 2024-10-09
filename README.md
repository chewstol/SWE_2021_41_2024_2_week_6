# SWE_2021_41_2024_2_week_6
## Week 4 Assignment
https://github.com/chewstol/SWE_2021_41_2024_2_week_4
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
First, check given number isHappy in one loop.  If it is not Happy in first loop, add it's result in 'loops'.  Do it until result is 1 or get result that is same with one in 'loops'. If it corresponds to the former, it is happy, and if it corresponds to the latter, it is not happy.
## Week 5 Assignment
<pre>
  <code>
    cat /etc/os-release
  </code>
</pre>
>I did it in my container. First, docker start ubuntu-container, and after that, cat /etc/os-release. It did well.
<pre>
  <code>
    git --version
  </code>
</pre>
>I did it in my container. First, docker start ossp-container, and after that, git --version. It did well, too.
<pre>
  <code>
    python3 --version
  </code>
</pre>
>I did it in my container. First, docker start ossp-container, and after that, python3 --version. It did well, too.
<pre>
  <code>
    docker inspect --format="{{ .HostConfig.Binds }}" ossp_container
  </code>
</pre>
