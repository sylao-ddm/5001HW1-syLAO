Please type Ctrl+Alt+T to enter Ubuntu Terminal and then try the bash scripts in the test file downloadable from this github.

The bash scripts are also shown here below and in the pdf report file submitted via canvas.

Thank you.

--------------------------------------------
The beginning of the report :

1) Check OS version :
     bash scripts:
          lsb_release -a
          hostnamectl
          uname -a

2) Check bash version :
     bash script :
          Bash --version

3) Check libraries or packages installed :
     bash script :
          apt list –installed
--------------------------------------------
Question 1 :

2) free -m  :  This is command for checking the total amount free and used physical and swap memory in  the system, as well as the buffers and caches used  by the kernel, with amount of memory displayed in mebibytes.  
      
   lshw -short : This is command for reporting detailed and brief information about multiple different hardware units such as cpu,  memory, disk, usb controllers, network adapters etc.  

   lscpu  :  Command for reporting information about the cpu and processing units.  
--------------------------------------------
Question 2 - Bash script :
   
script to create 100 folders named " DDM1, DDM2, ... , DDM100 " :
        
           #!/bin/bash ; for i in {1..100} ; do mkdir DDM$i ; done
    
script to generate a text file, "time_till_now.txt", in which the content is " nanoseconds since 1970-01-01 00:00:00 UTC: < XXXXXXXXXXXXXXXXXXX > for each of the 100 folders :

           for i in {1..100}; do echo "nanoseconds since 1970-01-01 00:00:00 UTC: < $(date +%s%N) >" > DDM$i/time_till_now.txt ; done
--------------------------------------------
Question 3 - Regular expression :

1) bash script : 
           grep -e 'blockID="i[0-9]\+"' -e 'blockID="g[0-9]\+"' blocklist.xml

2) bash script :

           grep -E 'id="\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Za-z]{2,6}\b"' blocklist.xml





