# BEMS-hourly-values
Program to post-process and visualize data from BEMS (Building Energy Management System), including calculating hourly values from sub-hourly logging, handling gaps, correcting for daylight saving time, and synchronizing the time of multiple logged parameters

### Key features
- Can handle a virtually unlimited number of logged parameters, each of which have independent time stamps. You simply paste two columns of data for each parameter into sheet 'Input'. The first column is the date/time (Excel format), and the second column is the logged data value.
- The output synchronizes the time-stamps of input parameters, and then calculates hourly statistics such as hour-mean or number of observations per hour.
- Can handle any logger interval, up to one hour. The logger interval need not be constant. BEMS systems typically have a logger interval of 5 or 10 minutes, sometimes only hourly.
- Can correct for Daylight Saving Time (DST) if you wish. Output is always in standard time (e.g. UTC+1 in Europe), but with an additional column for DST hour of day, so that you can correctly assess time schedules.
- Can calculate hourly energy use (e.g. average Watts during hour) from cumulative logged data (Wh electricity meter).
- Can calculate weighted averages or sums of input parameters, e.g. area-weighted temperature in a building. Input the weights (e.g. zone area) for each parameter in row 1 above the parameter's date/time column.
- Carpet plot to visualize calculated hourly output.

### Installation and activation
- Simply download the spreadsheet file and open it in Microsoft Excel. No installation or registration is needed.
- However, this is a Visual Basic macro-enabled spreadhseet. You must activate macros for it to function: 
  - When you open the file for the first time in Excel, you will see a yellow bar at the top of the window, with the message *"PROTECTED VIEW Be careful... [Enable Editing]"*. Click on the 'Enable Editing' button. 
  - Next, depending on the security settings on your installation of Microsoft Excel, a red bar may appear at the top of the window, with the message *"BLOCKED CONTENT Macros in this document have been disabled..."*. This can be solved by moving the file to a directory on your PC that you designate for files that you trust, then open the file in Excel. To designate a 'trusted directory', click on **File > Options > Trust Center > Trust Center Settings > Trusted Locations > Add new location**, then browse to a directory, e.g. C:\TEMP\. Finally check that **Trust Center Settings > Trusted Documents > Disable Trusted Documents**  is not ticked.
  - When macros are properly activated, **BEMS-hourly-values** shows a small square splash-screen when you open the file. This splash screen shows the licence info, and advises you if an update is available for download from GitHub. Simply press 'Close' button to close the splash-screen. 
  - If still no splash-screen appears, then you might be able to fix it by menu option **File > Options > Trust Center > Trust Center Settings > Macro Settings > Disable all macros with notification**, which is a suitable level of security.
  
### License & warranty
- Distributed under the GLP v3 lisence (https://www.gnu.org/licenses/gpl-3.0.en.html). Users of this software shall attribute its use in their reports/publications with an appropriate autohor citation and URL to this site.
- Provided without warranty of any kind.

### Author & copyright
© Peter.Schild@OsloMet.no
