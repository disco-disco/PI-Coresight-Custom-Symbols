## Line Chart symbol for PI Coresight 2016 R2.

This symbol is a work in progress.

## To deploy the symbol: 

1. In Windows Explorer, navigate to the "%PIHOME%\Coresight\Scripts\app\editor\symbols\ext" on your PI Coresight web server; typically, it's located in "C:\Program Files\PIPC\Coresight\Scripts\app\editor\symbols\ext".
If this folder doesn't exist, create it.

2. Place the following symbol files to the .\ext folder

	*sym-amcharts-linechart-template.html*
	
	*sym-amcharts-linechart-config.html*
	
	*sym-amcharts-linechart.js*

3. Place *LineChart.png* to the .\ext\Icons directory (create if it doesn't exist)
4. Place the Underscore library (*underscore-min.js*) to the .\ext\libraries (create if doesn't exist). The latest version of Underscore can be downloaded from http://underscorejs.org/.
5. Place the amCharts libraries (*amcharts.js*, *dark.js* and *serial.js*) to the .\ext\libraries folder.
6. Run iisreset


To convert this symbol to PI Vision 2017, replace the last line in the sym-amcharts-linechart.js file with *})(window.PIVisualization)*;


I.e. 
})(window.Coresight); => })(window.PIVisualization);