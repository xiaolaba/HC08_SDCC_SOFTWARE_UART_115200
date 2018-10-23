# HC08_SDCC_SOFTWARE_UART_115200  
HC08 core, software UART and timing calculation  
spreadsheet, ![HC08_baud_padding_calculation.xlsx](HC08_baud_padding_calculation.xlsx)  
  

formula  
ticks = CPU_MHz / baud * 10^6  
padding = ticks - tick  
x = padding / 3  
  



```
2018/OCT-22					
HC08 core					
xiaolaba					
					
CPU_MHz	baud	ticks	tick	padding	x
3.2	9600	333.33 	20	313.33 	104 
3.2	19200	166.67 	20	146.67 	49 
3.2	28800	111.11 	20	91.11 	30 
3.2	38400	83.33 	20	63.33 	21 
3.2	48000	66.67 	20	46.67 	16 
3.2	57600	55.56 	20	35.56 	12 
3.2	67200	47.62 	20	27.62 	9 
3.2	76800	41.67 	20	21.67 	7 
3.2	86400	37.04 	20	17.04 	6 
3.2	96000	33.33 	20	13.33 	4 
3.2	105600	30.30 	20	10.30 	3 
3.2	115200	27.78 	20	7.78 	3 
					
CPU_MHz	baud	ticks	tick	padding	x
3.2	9600	333.33 	9	324.33 	108 
3.2	19200	166.67 	9	157.67 	53 
3.2	28800	111.11 	9	102.11 	34 
3.2	38400	83.33 	9	74.33 	25 
3.2	48000	66.67 	9	57.67 	19 
3.2	57600	55.56 	9	46.56 	16 
3.2	67200	47.62 	9	38.62 	13 
3.2	76800	41.67 	9	32.67 	11 
3.2	86400	37.04 	9	28.04 	9 
3.2	96000	33.33 	9	24.33 	8 
3.2	105600	30.30 	9	21.30 	7 
3.2	115200	27.78 	9	18.78 	6 
					
					
CPU_MHz	baud	ticks	tick	padding	x
8	9600	833.33 	9	824.33 	275 
8	19200	416.67 	9	407.67 	136 
8	28800	277.78 	9	268.78 	90 
8	38400	208.33 	9	199.33 	66 
8	48000	166.67 	9	157.67 	53 
8	57600	138.89 	9	129.89 	43 
8	67200	119.05 	9	110.05 	37 
8	76800	104.17 	9	95.17 	32 
8	86400	92.59 	9	83.59 	28 
8	96000	83.33 	9	74.33 	25 
8	105600	75.76 	9	66.76 	22 
8	115200	69.44 	9	60.44 	20 
					
					
CPU_MHz	baud	ticks	tick	padding	x
8	9600	833.33 	20	813.33 	271 
8	19200	416.67 	20	396.67 	132 
8	28800	277.78 	20	257.78 	86 
8	38400	208.33 	20	188.33 	63 
8	48000	166.67 	20	146.67 	49 
8	57600	138.89 	20	118.89 	40 
8	67200	119.05 	20	99.05 	33 
8	76800	104.17 	20	84.17 	28 
8	86400	92.59 	20	72.59 	24 
8	96000	83.33 	20	63.33 	21 
8	105600	75.76 	20	55.76 	19 
8	115200	69.44 	20	49.44 	16 


```  
  
    
![HC08_blink_schematic.jpg](HC08_blink_schematic.jpg)  
  
![putty_test_done.JPG](putty_test_done.JPG)  
