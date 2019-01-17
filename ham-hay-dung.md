# DATE AND TIME FUNCTIONS

DATE(<year>, <month>, <day>)	Returns the specified date in datetime format.
 
DATEVALUE(date_text)	Converts a date in the form of text to a date in datetime format

DAY(<date>)	Returns the day of the month, a number from 1 to 31.
 
EDATE(<start_date>, <months>)	Returns the date that is the indicated number of months before or after the start date. Use EDATE to calculate maturity dates or due dates that fall on the same day of the month as the date of issue

EOMONTH(<start_date>, <months>)	Returns the date in datetime format of the last day of the month, before or after a specified number of months. Use EOMONTH to calculate maturity dates or due dates that fall on the last day of the month.

HOUR(<datetime>)	Returns the hour as a number from 0 (12:00 A.M.) to 23 (11:00 P.M.).

MINUTE(<datetime>)	Returns the minute as a number from 0 to 59, given a date and time value.

MONTH(<datetime>)	Returns the month as a number from 1 (January) to 12 (December).

NOW()	Returns the current date and time in datetime format.

SECOND(<time>)	Returns the seconds of a time value, as a number from 0 to 59

TIME(hour, minute, second)	Converts hours, minutes, and seconds given as numbers to a time in datetime format.

TIMEVALUE(time_text)	Converts a time in text format to a time in datetime format.

TODAY()	Returns the current date.

WEEKDAY(<date>, <return_type>)	Returns a number from 1 to 7 identifying the day of the week of a date. By default the day ranges from 1 (Sunday) to 7 (Saturday).

WEEKNUM(<date>, <return_type>)	Returns the week number for the given date and year according to the specified convention. The week number indicates where the week falls numerically within a year.

YEAR(<date>)	Returns the year of a date as a four digit integer in the range 1900-9999.

YEARFRAC(<start_date>, <end_date>, <basis>)	Calculates the fraction of the year represented by the number of whole days between two dates. Use the YEARFRAC worksheet function to identify the proportion of a whole year's benefits or obligations to assign to a specific term.
 

# INFORMATION FUNCTIONS

ISBLANK(<value>)	Checks whether a value is blank, and returns TRUE or FALSE.

ISERROR(<value>)	Checks whether a value is an error, and returns TRUE or FALSE.

ISLOGICAL(<value>)	Checks whether a value is a logical value, (TRUE or FALSE), and returns TRUE or FALSE.

ISNONTEXT(<value>)	Checks whether a value is not text (blank cells are not text), and returns TRUE or FALSE.

ISNUMBER(<value>)	Checks whether a value is a number, and returns TRUE or FALSE.

ISTEXT(<value>)	Checks whether a value is text, and returns TRUE or FALSE.
 

# FILTER AND VALUE FUNCTIONS

ALL(<table_or_column>)	Returns all the rows in a table, or all the values in a column, ignoring any filters that might have been applied.

ALLEXCEPT(<table>,column1>,<column2>,…)	Overrides all context filters in the table except filters that have been applied to the specified columns.

BLANK()	Returns a blank.

CALCULATE(<expression>,<filter1>,<filter2>…)	Evaluates an expression in a context that is modified by the specified filters.

CALCULATETABLE( <expression>, <filter1>, <filter2>,…)	Evaluates a table expression in a context modified by filters.

DISTINCT(<column>)	Returns a one-column table that contains the distinct values from the specified column.

EARLIER(<column>, <number>)	Returns the current value of the specified column in an outer evaluation pass of the mentioned column.

EARLIEST(<table_or_column>)	Returns the current value of the specified column in an outer evaluation pass of the mentioned column

FILTER(<table>,<filter>)	Returns a table that represents a subset of another table or expression.

RELATED(<column>)	Returns a related value from another table

RELATEDTABLE(<table>)	Follows an existing relationship, in either direction, and returns a table that contains all matching rows from the specified table.

VALUES(<column>)	Returns a one-column table that contains the distinct values from the specified column. This function is similar to 

DISTINCT function, but VALUES function can also return Unknown member

ALLNONBLANKROW(?)	Returns all the rows, except for blank rows, in a table or column, and disregards any context filters that might exist.

FIRSTNONBLANK(<column>,<expression>)	Returns the first non-blank values in column, filtered by expression.
 

# LOGICAL FUNCTIONS

AND(<logical1>,<logical2>,…)	Checks whether all arguments are TRUE, and returns TRUE if all arguments are TRUE.

FALSE()	Returns the logical value FALSE.

IF(logical_test>,<value_if_true>, value_if_false)	Checks if a condition provided as the first argument is met. Returns one value if the condition is TRUE, and returns another value if the condition is FALSE.

IFERROR(value, value_if_error)	Returns value_if_error if the first expression is an error and the value of the expression itself if otherwise.

NOT(<logical>)	Changes FALSE to TRUE, or TRUE to FALSE.

TRUE()	Returns the logical value TRUE.

OR(<logical1>,<logical2>,…)	Checks whether one of the arguments is TRUE to return TRUE. The function returns FALSE if all arguments are FALSE
 

# MATH AND TRIG FUNCTIONS

ABS(<number>)	Returns the absolute value of a number.

CEILING(<number>, <significance>)	Rounds a number up, to the nearest integer or to the nearest multiple of significance.

EXP(<number>)	Returns e raised to the power of a given number. The constant e equals 2.71828182845904, the base of the natural logarithm.

FACT(<number>)	Returns the factorial of a number, equal to the series 1*2*3*...* , ending in the given number.

FLOOR(<number>, <significance>)	Rounds a number down, toward zero, to the nearest multiple of significance.

INT(<number>)	Rounds a number down to the nearest integer.

LN(<number>)	Returns the natural logarithm of a number. Natural logarithms are based on the constant e (2.71828182845904).

LOG(<number>,<base>)	Returns the logarithm of a number to the base you specify.

LOG10(<number>)	Returns the base-10 logarithm of a number.

MOD(<number>, <divisor>)	Returns the remainder after a number is divided by a divisor. The result always has the same sign as the divisor.

MROUND(<number>, <multiple>)	Returns a number rounded to the desired multiple.

PI()	Returns the value of Pi, 3.14159265358979, accurate to 15 digits.

POWER(<number>, <power>)	Returns the result of a number raised to a power.

QUOTIENT(<numerator>, <denominator>)	Performs division and returns only the integer portion of the division result. Use this function when you want to discard the remainder of division.

ROUND(<number>, <num_digits>)	Rounds a number to the specified number of digits.

ROUNDDOWN(<number>, <num_digits>)	Rounds a number down, toward zero.

ROUNDUP(<number>, <num_digits>)	Rounds a number up, away from 0 (zero).

SIGN(<number>)	Determines the sign of a number, the result of a calculation, or a value in a column. The function returns 1 if the number is positive, 0 (zero) if the number is zero, or -1 if the number is negative.

SQRT(<number>)	Returns the square root of a number.

TRUNC(<number>,<num_digits>)	Truncates a number to an integer by removing the decimal, or fractional, part of the number.
[vb] RAND()	Returns a random number greater than or equal to 0 and less than 1, evenly distributed. The number that is returned changes each time the cell containing this function is recalculated.
[vb] RANDBETWEEN(<bottom>,<top>)	Returns a random number between the numbers you specify
 

# STATISTICAL FUNCTIONS

AVERAGE(<column>)	Returns the average (arithmetic mean) of all the numbers in a column.

AVERAGEA(<column>)	Returns the average (arithmetic mean) of the values in a column. Handles text and non-numeric values.

AVERAGEX(<table>, <expression>)	Calculates the average (arithmetic mean) of a set of expressions evaluated over a table

COUNT(<column>)	The COUNT function counts the number of cells in a column that contain numbers.

COUNTA(<column>)	The COUNTA function counts the number of cells in a column that are not empty.

COUNTAX(<table>, <expression>)	The COUNTAX function counts nonblank results when evaluating the result of an expression over a table.

COUNTBLANK(<column>)	Counts the number of blank cells in a column.

COUNTROWS(<table>)	The COUNTROWS function counts the number of rows in the specified table, or in a table defined by an expression.

COUNTX(<table>, <expression>)	Counts the number of rows that contain a number or an expression that evaluates to a number, when evaluating an expression over a table.

MAX(<column>)	Returns the largest numeric value in a column.

MAXA(<column>)	Returns the largest value in a column. Logical values and blanks are counted.

MAXX(<table>, <expression>)	Evaluates an expression for each row of a table and returns the largest numeric value.

MIN(<column>)	Returns the smallest numeric value in a column. Ignores logical values and text.

MINA(<column>)	Returns the smallest value in a column, including any logical values and numbers represented as text.

MINX(<table>, < expression>)	Returns the smallest numeric value that results from evaluating an expression for each row of a table.

SUM(<column>)	Adds all the numbers in a column.

SUMX(<table>, <expression>)	Returns the sum of an expression evaluated for each row in a table.
 

# TEXT FUNCTIONS

CODE(<text>)	Returns a numeric code for the first character in a text string, in the character set used by your computer.

CONCATENATE(<text1>, <text2>,…)	The CONCATENATE function joins multiple text strings into one text string. The joined items can be text, numbers or Boolean values represented as text, or a combination of those items. You can also use a column reference if the column contains appropriate values.

EXACT(<text1>,<text2>)	Compares two text strings and returns TRUE if they are exactly the same, FALSE otherwise. EXACT is case-sensitive but ignores formatting differences. You can use EXACT to test text being entered into a document.

FIND(<find_text, within_text, start_num)	Returns the starting position of one text string within another text string. FIND is case-sensitive.

FIXED(<number>, <decimals>, <no_commas>)	Rounds a number to the specified number of decimals and returns the result as text. You can specify that the result be returned with or without commas.

LEFT(<text>, <num_chars>)	Returns the specified number of characters from the start of a text string.

LEN(<text>)	Returns the number of characters in a text string.

LOWER(<text>)	Converts all letters in a text string to lowercase.

MID(<text>, <start_num>, <num_chars>)	Returns a string of characters from the middle of a text string, given a starting position and length.

REPLACE(<old_text>, <start_num>, <num_chars>, <new_text>)	REPLACE replaces part of a text string, based on the number of characters you specify, with a different text string.

REPT(<text>, <num_times>)	Repeats text a given number of times. Use REPT to fill a cell with a number of instances of a text string

RIGHT(<text>, <num_chars>)	RIGHT returns the last character or characters in a text string, based on the number of characters you specify.

SEARCH(<search_text>, <within_text>, [start_num])	Returns the number of the character at which a specific character or text string is first found, reading left to right. Search is case-sensitive.

SUBSTITUTE(<text>, <old_text>, <new_text>, <instance_num>)	Replaces existing text with new text in a text string.

TRIM(<text>)	Removes all spaces from text except for single spaces between words.

UPPER (<text>)	Converts a text string to all uppercase letters

VALUE(<text>)	Converts a text string that represents a number to a number.

FORMAT(<value>, <format_string>)	Converts a value to text according to the specified format.
 

# TIME INTELLIGENCE FUNCTIONS

CLOSINGBALANCEMONTH(<expression>,<dates>,<filter>)	Evaluates the specified expression at the calendar end of the given month. The given month is calculated as the month of the latest date in the dates argument, after applying all filters.

CLOSINGBALANCEQUARTER(<expression>,<dates>,<filter>)	Evaluates the specified expression at the calendar end of the given quarter. The given quarter is calculated as the quarter of the latest date in the dates argument, after applying all filters.

CLOSINGBALANCEYEAR(<expression>,<dates>,<filter>)	Evaluates the specified expression at the calendar end of the given year. The given year is calculated as the year of the latest date in the dates argument, after applying all filters.

DATESINPERIOD(<date_column>,<start_date>,<number_of_intervals>,<intervals>)	Returns a table of dates that can be found in the specified date column beginning with the start date and continuing for the specified number of intervals.

DATESBETWEEN(<column>,<start_date>,<end_date>	Returns a table of dates that can be found in the specified date column beginning with the start date and ending with the end date.

DATEADD(<date_column>,<number_of_intervals>,<interval>)	Returns a table that contains a column of dates, shifted either forward in time or back in time from the dates in the specified date column.

FIRSTDATE (<datecolumn>)	Returns the first date in the current context for the specified Date_Column.

LASTDATE (<datecolumn>)	Returns the last date in the current context for the specified Date_Column.

LASTNONBLANK (<datecolumn>,<expression>)	?

STARTOFMONTH (<date_column>)	Returns the first day of the month in the specified date column.

STARTOFQUARTER (<date_column>)	Returns the first day of the quarter in the specified date column.

STARTOFYEAR(<date_column>[,<YE_date>])	Returns the first day of the year in the specified date column.

ENDOFMONTH(<date_column>)	Returns the last day of the month in the specified date column.

ENDOFQUARTER(<date_column>)	Returns the last day of the quarter in the specified date column.

ENDOFYEAR(<date_column>)	Returns the last day of the year in the specified date column.

PARALLELPERIOD(<date_column>,<number_of_intervals>,<intervals>)	This function moves the specified number of intervals and then returns all contiguous full months which contain any values after that shift. Gaps between the first and last dates are filled in, and months are also filled in.

PREVIOUSDAY(<date_column>)	Returns the previous day date from date_column.

PREVIOUSMONTH(<date_column>)	Returns the set of dates in the previous month from date_column.

PREVIOUSQUARTER(<date_column>)	Returns the set of dates in the previous quarter from date_column.

PREVIOUSYEAR(<date_column>)	Returns the set of dates in the previous year from date_column.

NEXTDAY(<date_column>)	Returns the next day date from date_column.

NEXTMONTH(<date_column>)	Returns the set of dates in the next month from date_column.

NEXTQUARTER (<date_column>)	Returns the set of dates for the next quarter from date_column

NEXTYEAR(<date_column>[,<YE_date>])	Returns the set of dates for the next year from date_column.

DATESMTD(<date_column>)	Returns the subset of dates, from date_column, for the interval that starts at the first day of the month and 
ends at the latest date in the specified dates column for the month that is the corresponding month of the latest date.

DATESQTD (<date_column>)	Returns the subset of dates, from date_column, for the interval that starts at the first day of the quarter and ends at the latest date in the specified dates column for the quarter that is the corresponding quarter of the latest date.

DATESYTD (<date_column> [,<YE_date>])	Returns the subset of dates, from date_column, for the interval that starts the first day of the year and ends at the latest date in the specified dates column for the quarter that is the corresponding quarter of the latest date.

SAMEPERIODLASTYEAR() - ?	?

OPENINGBALANCEMONTH(<expression>,<dates>,<filter>)	Evaluates the specified expression at the calendar end of the month prior the given month. The given month is calculated as the month of the latest date in the dates argument, after applying all filters.

OPENINGBALANCEQUARTER(<expression>,<dates>,<filter>)	Evaluates the specified expression at the calendar end of the quarter prior to the given quarter. The given quarter is calculated as the quarter of the latest date in the dates argument, after applying all filters.
OPENINGBALANCEYEAR(<expression>,<dates>,<filter>)	Evaluates the specified expression at the calendar end of the year prior to the given year. The given year is calculated as the year of the latest date in the dates argument, after applying all filters.
TotalMTD(<expression>,<dates>,<filter>)	Evaluates the specified expression for the interval that starts at the first day of the month and ends at the latest date in the specified dates column, after applying all filters.
TotalQTD(<expression>,<dates>,<filter>)	Evaluates the specified expression for the interval that starts at the first day of the quarter and ends at the latest date in the specified dates column, after applying all filters.
TotalYTD(<expression>,<dates>,<filter>)	Evaluates the specified expression for the interval that starts at the first day of the year and ends at the latest date in the specified dates column, after applying all filters.
