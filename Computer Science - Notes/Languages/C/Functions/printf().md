printf( “format-string”, [ arg1, arg2, ... ] );  
format-string:  
Composed of literals and format specifiers. Arguments are required only if there are format  
specifiers in the format string. Format specifiers include: flags, width, precision, and conversion  
characters in the following sequence:  
% [flags] [width] [.precision] conversion-character( square brackets denote optional parameters )  
flags:  
- : left-justify ( default is to right-justify )  
+ : output a plus ( + ) or minus ( - ) sign for a numerical value  
0 : forces numerical values to be zero-padded ( default is blank padding )  
, : comma grouping separator (for numbers > 1000)  
width:  
Specifies the field width for outputting the argument and represents the minimum number of  
characters to be written to the output. Include space for expected commas and a decimal point in  
the determination of the width for numerical values.  
precision:  
Used to restrict the output depending on the conversion. It specifies the number of digits of  
precision when outputting floating-point values or the length of a substring to extract from a String.  
Numbers are rounded to the specified precision.  
conversion-characters:  
d : decimal integer[byte, short, int, long]  
f : floating-point number [float, double]  
c : character, Capital C will uppercase the letter  
Examples:  
double dblTotal=27.515;  
int intValue=22;  
printf("Total is: $%,.2f\n", dblTotal); //Total is: $27.52  
printf("Total: %-10.1f: ", dblTotal); //Total: 27.5bbbbbb  
printf("%4d", intValue); // 22bb  
rounded to 2 decimal places, comma inserted if needed  
left adjust, rounded to 1 decimal place, double data value, 10 spaces total used  
4 spaces total used, automatically right justified, integer value