# 5001HW1-syLAO

Bash Scripts for:

Question 2:

#!/bin/bash ; for i in {1..100} ; do mkdir DDM$i ; done

for i in {1..100}; do echo "nanoseconds since 1970-01-01 00:00:00 UTC: < $(date +%s%N) >" > DDM$i/time_till_now.txt ; done


Question 3:

cat blocklist.xml | grep
