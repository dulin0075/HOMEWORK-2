# **第二次作业** #

----------


# P5 #
回顾在1.4节中的车队的类比。假定传播速度为100km/h。a.假定车队旅行150km：在一个收费站前面开始，通过第二个收费站，并且正好在第三个收费站后面结束。其端到端时延是多少？ b.重复（a）,现在假定车队中有8辆汽车而不是10辆。

a.车队通过一个收费站时间t1=10*12s=2min；从一个收费站到另一个收费站时间t2=75/100h=0.75h；所以时延t=3t1+2t2=96min。

b.t1'=8*12s=1.6min；时延t'=94.8min。

----------
# P12 #
 —台分组交换机接收一个分组并决定该分组应当转发的出链路。当某分组到达时，另一个分组正在该出链路上被发送到一半，还有4个其他分组正等待传输。这些分组以到达的次序传输。假定所有分组是1500字节并且链路速率是2Mbps。该分组的排队时延是多少？在更一般的情况下，当所有分组的长度是L，传输速率是R，当前正在传输的分组已经传输了x比特，并且已经在队列中有n个分组，其排队时延是多少？

有一个完整分组的排队时延为（1500*8b）/2Mbps=0.6ms；4.5个分组的总排队时延为2.7ms；一般情况下，排队时延为Ln/R+（L-x）/R。

----------
# P13 #
 a.假定有N个分组同时到达一条当前没有分组传输或排队的链路。每个分组长为L，链路传输速率为R。对N个分组而言.其平均排队时延是多少？ b.现在假定每隔LN/R秒有N个分组同时到达链路。一个分组的平均排队时延是多少？ 

a.第一个分组的排队时延为0，第二个为L/R，第三个为2L/R，……，第N个为（N-1)/R；所以平均排队时延为(L/R + 2L/R + … + (N-1)L/R) / N = (N-1)L/2R。

b.当下一批 N 个分组到达时，上一批已经传完，因此平均排队时延为 (N-1)L/2R。


