# BEMS-hourly-values
Program to post-process and visualize data from BEMS (Building Energy Management System), including calculating hourly values from sub-hourly logging, handling gaps, correcting for daylight saving time, and synchronizing the time of multiple logged parameters

### Key features
- This is a Visual Basic macro-enabled spreadhseet. You must activate macros for it to function.
- Can handle a virtually unlimited number of logged parameters, each of which have independent time stamps. You simply paste two columns of data for each parameter into sheet 'Input'. The forst column is the time, and the second column is the logged data.
- The output synchronizes the input parameters, and calculates hourly statistics.
- Can handle any logger interval, up to one hour. The logger interval need not be constant. BEMS systems typically have a logger interval of 5 or 10 minutes, sometimes only hourly.
- Can correct for Daylight Saving Time (DST) if you wish. Output is always in standard time (e.g. UTC+1 in Europe), but with an additional column for DST hour of day, so that you can correctly assess time schedules.
- Can calculate hourly energy use (e.g. average Watts during hour) from cumulative logged data (Wh electricity meter).
- Can calculate weighted averages or sums of input parameters, e.g. area-weighted temperature in a building. Input the weights (e.g. zone area) for each parameter in row 1 above the parameter's date/time column.
- Carpet plot to visualize calculated hourly output.

### License & warranty
- Distributed under the GLP v3 lisence (https://www.gnu.org/licenses/gpl-3.0.en.html). Users of this software shall attribute its use in their reports/publications with an appropriate autohor citation and URL to this site.
- Provided without warranty of any kind.

### Author & copyright
© Peter.Schild@OsloMet.no
