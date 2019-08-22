# Prediction-of-yield-rate-of-Wafer-production-parameters

I do the following process to analyse and train the processed datas with several machine learning models.
1. The data are sotred in seperate files grouped by digit number include 6, 7, 8, 11, 12, 15 and ann as extsion filenames and have 4-digit_2-digit as major filenames. For example,1886_25.ann, 1886_25.6 etc. You can see the files in the directory named  sample_raw_files. I merge all the data files with MergeDataBase.ipynb and produce the output file raw.csv. Make some modification to produce to get out.csv and out_abnomal.csv which represent normal yield datas and abnormal yield datas respectively.
2. First observe the raw data by visualizing datas using df.plot and find there are 2 phase of stable datas and transient datas. Then use 2batch_normal_sean.ipynb and 2batch_abnormal_sean.ipynb to get rid of ouliers and get 2 phase of stable datas by groupby and agg function, and then get 2batch_P_normal.csv and 2batch_P_abnormal.csv.
3. Use "Randomforest-Project2-Upsampling-sean.ipynb", "SVM-Project2-Upsampling-sean.ipynb" to train and verify datas. Comes up that Randomforest get better precision.
