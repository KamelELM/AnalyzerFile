# AnalyzerFile
File Analyzer For data from timepix3

The FileAnalizer project is used for accelerated the treatment of the timepix3. 

All data are storage in ".txt" file, 
the data are separated by tabs arranged in columns
Column 1 : CoordinatesXY
Column 2 : ToA_Coarse
Column 3 : ToA_Fine
Column 4 : Tot

The Coordinates X and Y are determined by : CoordinatesXY = Y * 256 + X
The Time_Stamp is find by : Time_Stamp (ToA_Coarse * F_carte) - (ToA_Fine * F_timepix3)
F_timepix3 0.0000000015625
F_carte =  0.000000025
