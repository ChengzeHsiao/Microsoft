TCP ���ԣ�

���շ���ntttcp -r -p 80 -a 6 -t 60 -cd 5 -wu 5 -v -xml c:\bench.xml  -m 1,0,10.10.10.12 1,1,10.10.10.12


���ͷ���ntttcp -s -p 80 -a -t 60 -cd 5 -wu 5 -m 1,0,10.10.10.12 1,1,10.10.10.12


UDP ���ԣ�

���շ���ntttcp �Cr �Cu -p 80 �Ct 60 �Ccd 5 �Cwu 5 �Cv �Cxml c:\bench.xml -m 1,0,10.10.10.12 1,1,10.10.10.12



���ͷ���ntttcp -s �Cu -p 80 -t 60 -cd 5 -wu 5 -m 1,0,10.10.10.12 1,1,10.10.10.12

�ο����ף�
https://aws.amazon.com/cn/premiumsupport/knowledge-center/network-throughput-benchmark-windows-ec2/?nc1=h_ls
