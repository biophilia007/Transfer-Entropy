# Transfer-Entropy
The code for calculating the transfer entropy between various brain regions in the BOLD-EPI sequence was implemented using the Kozachenko-Leonenko and Kraskov-Stögbauer-Grassberger from the Java Information Dynamics Toolkit (JIDT).
1. You need to prepare the preprocessed BOLD-EPI data.  
2. You need to extract the time series for each brain region in the atlas you are using and organize them in a format where rows represent brain region labels and columns represent time series. Save this data as a `ROISignals_*.mat` file.  
3. Define the history length 'k', target history length 'l', and delay 'delay' based on the TR time of the data and the number of time points.  
4. Please note that negative values in Transfer Entropy (TE) are meaningless. For a detailed explanation of the underlying principles, you can refer to the video tutorial available at [https://github.com/jlizier/jidt](https://github.com/jlizier/jidt). Therefore, it is necessary to convert any negative TE values to 0.
Our code utilizes the `infodynamics.jar` file from JIDT, so you must download this file first.
