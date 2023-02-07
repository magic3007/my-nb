# CPU Number

```bash
# 逻辑CPU数量和型号
cat /proc/cpuinfo | grep name | cut -f2 -d: | uniq -c

# 物理CPU数量
cat /proc/cpuinfo | grep "physical id" | sort | uniq | wc -l  
 
# 物理CPU内核的个数 (1个物理CPU里面有几个物理内核)
cat /proc/cpuinfo | grep "cpu cores" | uniq  
 
# 查看所有逻辑CPU的个数
cat /proc/cpuinfo | grep "processor" | wc -l
 
# 物理CPU中逻辑CPU的个数】（如果不使用超线程技术，则此值和物理CPU内核数量一致；不一致则为整倍数）
cat /proc/cpuinfo | grep 'siblings' | uniq
 
# 超线程（分别输出cpu cores和siblings数量，使用超线程则后者翻倍）
cat /proc/cpuinfo | grep -e "cpu cores" -e "siblings" | sort | uniq
```
