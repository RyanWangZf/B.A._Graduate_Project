## oracle_loader.py  
���ڴ�oracle database����ȡԭ���ݣ��洢Ϊcsv�ļ�  
extract data from Oracle database, saving as *.csv  

## match_RTDMD_CLIENT.py  
����ƥ��RTDMD�����CLIENTINFO�Ĳ��λ��  
matach RTDMD's location with CLIENTINFO  

## heatmap.py  
���ڻ����¹ʵĵص�ֲ�����
gaussian kernel density estimation ����¹ʷֲ������ܶȣ�
�����ֲ���ͼ  
use Kernel Density Estimation to fit the geographical probability distribution,
then paint the hear map  

## get_dtw_D.py  
��ÿ������365����������DTW����Ľ������
��Ϊ��һ���׾�����ڽӾ���(affinity matrix)  
get cross DTW distance matrix as the pre-computed affinity matrix  

## spec_cluster.py  
���ݵõ��ĵ�һ���ÿ�����dtw�������D��
��ÿ���������������ಢ�õ�ÿ������8����������  
do spectral clustering based on D matrix from get_dtw_D.py,
then get 8 typical time-series from every detection monitor's data.  

## last_dtw_cluster.py  
�ɵ�һ�����õ��ĵ������м��㽻��������D��
����D���׾��࣬���յõ����в����������е�
10����������  
get 10 typical time series from 8*number of detection monitor's typical time series
 by spectral clustering, too.  

## report_ser_match.py  
ƥ���¹ʷ���������Ĳ�����к�  
match the nearest monitor of every failure report  

## ts_report_stats.py  
ƥ��10�������������¹ʷ����ز�����У�չʾ��ͬ���еķ��նȲ���  
match 2015 failure reports with every 10 typical time series, show the stats results.  

## 2016_report_ts.py  
ƥ��2016����¹�������10��ģ���ߣ���֤�߷���ģ������2016���Ƿ����Ϊ�߷���  
match 2016 failure reports with every 10 typical time series, show stats results to 
vertify whether or not the risky series in 2015 keep risky in 2016.  

## sampling_ts.py  
��2016�������������ȡ300�������У���֤���¹������Ƿ���ϸ߷���ģ����  
sampling over 300 series randomly and match with 10 typical time series, verifying if normal 
series match the risky series.  

