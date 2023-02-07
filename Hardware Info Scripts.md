# CPU Number

```bash
# number and types of logical CPUs
cat /proc/cpuinfo | grep name | cut -f2 -d: | uniq -c

# number of physical CPUs
cat /proc/cpuinfo | grep "physical id" | sort | uniq | wc -l  
 
# number of physical cores per physical CPU
cat /proc/cpuinfo | grep "cpu cores" | uniq
 
# number of all logical cores 
cat /proc/cpuinfo | grep "processor" | wc -l
 
# 物理CPU中逻辑CPU的个数 (如果不使用超线程技术，则此值和物理CPU内核数量一致；不一致则为整倍数）
cat /proc/cpuinfo | grep 'siblings' | uniq
 
# 超线程（分别输出cpu cores和siblings数量，使用超线程则后者翻倍）
cat /proc/cpuinfo | grep -e "cpu cores" -e "siblings" | sort | uniq
```
