

# Variable

**A variable is just a reference to a value. A variable does not contain
the value.**


::: {.cell .markdown}
`<b>`{=html}Syntax for assigning a reference to a value:
`</b>`{=html}`<br>`{=html}

variableName=Value
:::

::: {.cell .markdown}
`<b>`{=html}NOTE`</b>`{=html}: If there is space to the left and right
side of the variableName, then that space will be ignored
:::

::: {.cell .markdown}
`<b>`{=html}Points to follow, while creating variableNames`</b>`{=html}
`<br>`{=html} 1) The first character of a variableName should be an
alphabet of lower case (a-z), or it can be an alphabet of upper case
(A-Z), or an underscore (*) `<br>`{=html} 2) All the characters of the
variableName apart from the first character should be an alphabet of
lower case (a-z), or it can be an alphabet of upper case (A-Z), or an
underscore (*), or it can be a digit charcater(0-9) `<br>`{=html} 3) A
variableName cannot have space within it. `<br>`{=html} 4) A
variableName cannot have any special characters (!,@,\$,\#,%,\^,&,etc.)
`<br>`{=html} 5) A variableName is case sensitive (apple is not the same
as Apple)
:::

::: {.cell .code execution_count="1"}
``` {.python}
#The variable created below, is not valid as the first rule for variable creation is not being followed

007bond=25
```

::: {.output .error ename="SyntaxError" evalue="leading zeros in decimal integer literals are not permitted; use an 0o prefix for octal integers (<ipython-input-1-bf1173183aef>, line 1)"}
      File "<ipython-input-1-bf1173183aef>", line 1
        007bond=25
          ^
    SyntaxError: leading zeros in decimal integer literals are not permitted; use an 0o prefix for octal integers
:::
:::

::: {.cell .code execution_count="2"}
``` {.python}
# The variable created below, is valid as all the five rules of variable creation are being followed

bond007=25
```
:::

::: {.cell .code execution_count="3"}
``` {.python}
# Printing the value referenced by the variable- 'bond007'

bond007
```

::: {.output .execute_result execution_count="3"}
    25
:::
:::

::: {.cell .code execution_count="4"}
``` {.python}
#The variable created below, is not valid as the fourth rule for variable creation is not being followed

Devi@=26
```

::: {.output .error ename="NameError" evalue="name 'Devi' is not defined"}
    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    <ipython-input-4-2dea4554d1bb> in <module>
    ----> 1 Devi@=26

    NameError: name 'Devi' is not defined
:::
:::

::: {.cell .code execution_count="5"}
``` {.python}
# The variable created below, is valid as all the five rules of variable creation are being followed

Devi=26
```
:::

::: {.cell .code execution_count="6"}
``` {.python}
# The variable created below, is valid as all the five rules of variable creation are being followed

devi=27
```
:::

::: {.cell .code execution_count="7"}
``` {.python}
# Printing the value referenced by the variable- 'devi'

devi
```

::: {.output .execute_result execution_count="7"}
    27
:::
:::

::: {.cell .code execution_count="8"}
``` {.python}
# Printing the value referenced by the variable- 'Devi'

Devi
```

::: {.output .execute_result execution_count="8"}
    26
:::
:::

::: {.cell .code execution_count="9"}
``` {.python}
#The variable created below, is not valid as the third rule for variable creation is not being followed

Rohit Sharma=28
```

::: {.output .error ename="SyntaxError" evalue="invalid syntax (<ipython-input-9-4164e7058332>, line 1)"}
      File "<ipython-input-9-4164e7058332>", line 1
        Rohit Sharma=28
              ^
    SyntaxError: invalid syntax
:::
:::

::: {.cell .code execution_count="10"}
``` {.python}
# The variable created below, is valid as all the five rules of variable creation are being followed

RohitSharma=28
```
:::

::: {.cell .markdown}
If a Value does not have a reference in jupyter notebook, then the below
2 things will happen: `<br>`{=html} 1) The value will get printed
automatically `<br>`{=html} 2) Value will get deleted automatically
`<br>`{=html}
:::

::: {.cell .code execution_count="13"}
``` {.python}
# The below created value does not have a reference assigned to it

31
```

::: {.output .execute_result execution_count="13"}
    31
:::
:::

::: {.cell .code execution_count="14"}
``` {.python}
# The below created value does have a reference assigned to it

a=32
```
:::

::: {.cell .code execution_count="16"}
``` {.python}
# Printing the value referenced by the variable- 'a'

a
```

::: {.output .execute_result execution_count="16"}
    33
:::
:::

::: {.cell .markdown}
# Types of Values
:::

::: {.cell .markdown}
1\) Integer `<br>`{=html} 2) Float `<br>`{=html} 3) String `<br>`{=html}
4) Boolean `<br>`{=html}
:::

::: {.cell .markdown}
# 1) Integer {#1-integer}
:::

::: {.cell .markdown}
Integer is just a number without any decimal point
:::

::: {.cell .code execution_count="17"}
``` {.python}
# In the below code, we created a integer value 50

a=50
```
:::

::: {.cell .code execution_count="18"}
``` {.python}
type(a)
```

::: {.output .execute_result execution_count="18"}
    int
:::
:::

::: {.cell .code execution_count="19"}
``` {.python}
# In the below code, we created a integer value 0

b=0
```
:::

::: {.cell .code execution_count="20"}
``` {.python}
type(b)
```

::: {.output .execute_result execution_count="20"}
    int
:::
:::

::: {.cell .code execution_count="21"}
``` {.python}
# In the below code, we created a integer value -100

c=-100
```
:::

::: {.cell .code execution_count="22"}
``` {.python}
type(c)
```

::: {.output .execute_result execution_count="22"}
    int
:::
:::

::: {.cell .markdown}
# 2) Float {#2-float}
:::

::: {.cell .markdown}
Float is just a number with decimal point
:::

::: {.cell .code execution_count="23"}
``` {.python}
# In the below code, we created a float value -30.0

d=30.0
```
:::

::: {.cell .code execution_count="24"}
``` {.python}
type(d)
```

::: {.output .execute_result execution_count="24"}
    float
:::
:::

::: {.cell .code execution_count="25"}
``` {.python}
# In the below code, we created a float value 0.001

e=0.001
```
:::

::: {.cell .code execution_count="26"}
``` {.python}
type(e)
```

::: {.output .execute_result execution_count="26"}
    float
:::
:::

::: {.cell .code execution_count="27"}
``` {.python}
# In the below code, we created a float value -10.3

f=-10.3
```
:::

::: {.cell .code execution_count="28"}
``` {.python}
type(f)
```

::: {.output .execute_result execution_count="28"}
    float
:::
:::

::: {.cell .markdown}
# 3) String {#3-string}
:::

::: {.cell .markdown}
A string is just a collection of characters. Inorder to tell python that
you have a collection of characters, you need to surround that
collection with single quotes, double quotes, triple quotes.
`<br>`{=html} NOTE: The type of quote that you are starting with should
match with the type of quote that you are ending it.
:::

::: {.cell .code execution_count="29"}
``` {.python}
# In the below code, we created a string value - rishabhpant

g="rishabhpant"
```
:::

::: {.cell .code execution_count="30"}
``` {.python}
type(g)
```

::: {.output .execute_result execution_count="30"}
    str
:::
:::

::: {.cell .code execution_count="31"}
``` {.python}
# In the below code, we created a string value - bond007

h='bond007'
```
:::

::: {.cell .code execution_count="32"}
``` {.python}
type(h)
```

::: {.output .execute_result execution_count="32"}
    str
:::
:::

::: {.cell .code execution_count="33"}
``` {.python}
# In the below code, we created a string value - dollar$

j='''dollar$'''
```
:::

::: {.cell .code execution_count="34"}
``` {.python}
type(j)
```

::: {.output .execute_result execution_count="34"}
    str
:::
:::

::: {.cell .markdown}
`<b>`{=html} In the below code, the type of quote at the beginning of
the string value is not matching with the type of quote at the end of
the string value, because of which we would receive a error
`</b>`{=html}
:::

::: {.cell .code execution_count="36"}
``` {.python}

k="apple'
```

::: {.output .error ename="SyntaxError" evalue="EOL while scanning string literal (<ipython-input-36-7e321b2182e7>, line 1)"}
      File "<ipython-input-36-7e321b2182e7>", line 1
        k="apple'
                 ^
    SyntaxError: EOL while scanning string literal
:::
:::

::: {.cell .markdown}
# 4) Boolean {#4-boolean}
:::

::: {.cell .markdown}
True and False are called boolean values. The first character of the
boolean value needs to be in uppercase, while the rest of the characters
of your boolean value need to be in lower case.
:::

::: {.cell .code execution_count="37"}
``` {.python}
#The value created below is not a boolean,string,integer or float

x=true
```

::: {.output .error ename="NameError" evalue="name 'true' is not defined"}
    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    <ipython-input-37-fe79c7b8bd75> in <module>
    ----> 1 x=true

    NameError: name 'true' is not defined
:::
:::

::: {.cell .code execution_count="38"}
``` {.python}
# The value created below is a boolean value
x=True
```
:::

::: {.cell .code execution_count="39"}
``` {.python}
type(x)
```

::: {.output .execute_result execution_count="39"}
    bool
:::
:::

::: {.cell .code execution_count="40"}
``` {.python}
#The value created below is not a boolean,string,integer or float

y=TruE
```

::: {.output .error ename="NameError" evalue="name 'TruE' is not defined"}
    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    <ipython-input-40-07774d5fa91d> in <module>
    ----> 1 y=TruE

    NameError: name 'TruE' is not defined
:::
:::

::: {.cell .code execution_count="41"}
``` {.python}
# The value created below is a boolean value

y=True
```
:::

::: {.cell .code execution_count="42"}
``` {.python}
type(y)
```

::: {.output .execute_result execution_count="42"}
    bool
:::
:::

::: {.cell .code execution_count="43"}
``` {.python}
# The value created below is a boolean value

z=False
```
:::

::: {.cell .code execution_count="44"}
``` {.python}
type(z)
```

::: {.output .execute_result execution_count="44"}
    bool
:::
:::

::: {.cell .markdown}
# Understanding immutability
:::

::: {.cell .code execution_count="45"}
``` {.python}
# Here we have created a value of 50 and assigned a reference of "z" to it
z=50
```
:::

::: {.cell .markdown}
`<b>`{=html}Here we have created a value of 50 and assigned a reference
of \"z\" to it. Now, the variable \"z\" which was previously referencing
the value of 50, will now refer the value 51. The value 50 will not have
any variable referencing it. `</b>`{=html}
:::

::: {.cell .code execution_count="46"}
``` {.python}
z=51
```
:::

::: {.cell .code execution_count="47"}
``` {.python}
z
```

::: {.output .execute_result execution_count="47"}
    51
:::
:::

::: {.cell .markdown}
`<b>`{=html}NOTE: Integer, Float, String, Boolean are immutable types of
values. That means you cannot do any change in them.`</b>`{=html}
:::

::: {.cell .markdown}
# Type Conversion
:::

::: {.cell .markdown}
# 1) Integer to other types of values {#1-integer-to-other-types-of-values}
:::

::: {.cell .code execution_count="48"}
``` {.python}
# Here, we created a integer value of 50, and assigned a variable of "a" as a reference to it
a=50
```
:::

::: {.cell .markdown}
`<b>`{=html}Conversion to float: `</b>`{=html}`<br>`{=html} 1) Convert
the value to a real number `<br>`{=html} 2) Convert the real number to a
number with decimal `<br>`{=html}
:::

::: {.cell .code execution_count="49"}
``` {.python}
# Here, the value referenced by variable "a" is converted to float

a=float(a)
```
:::

::: {.cell .code execution_count="50"}
``` {.python}
a
```

::: {.output .execute_result execution_count="50"}
    50.0
:::
:::

::: {.cell .code execution_count="51"}
``` {.python}
b=-10
```
:::

::: {.cell .code execution_count="52"}
``` {.python}
# Here, the value referenced by variable "b" is converted to float

float(b)
```

::: {.output .execute_result execution_count="52"}
    -10.0
:::
:::

::: {.cell .markdown}
`<b>`{=html}If a Value does not have a reference in jupyter notebook,
then: `</b>`{=html}`<br>`{=html} 1) The value will get printed
automatically (while creating that value) `<br>`{=html} 2) Value will
get deleted automatically `<br>`{=html}
:::

::: {.cell .markdown}
`<b>`{=html}Conversion to string:`</b>`{=html} `<br>`{=html} 1) Surround
the value with quotes(single quote) `<br>`{=html}
:::

::: {.cell .code execution_count="53"}
``` {.python}
c=100
```
:::

::: {.cell .code execution_count="54"}
``` {.python}
type(c)
```

::: {.output .execute_result execution_count="54"}
    int
:::
:::

::: {.cell .code execution_count="55"}
``` {.python}
# Here, the value referenced by variable "c" is converted to string

d=str(c)
```
:::

::: {.cell .code execution_count="56"}
``` {.python}
d
```

::: {.output .execute_result execution_count="56"}
    '100'
:::
:::

::: {.cell .code execution_count="57"}
``` {.python}
e=40
```
:::

::: {.cell .code execution_count="58"}
``` {.python}
# Here, the value referenced by variable "e" is converted to bool

bool(e)
```

::: {.output .execute_result execution_count="58"}
    True
:::
:::

::: {.cell .code execution_count="59"}
``` {.python}
f=0
```
:::

::: {.cell .code execution_count="60"}
``` {.python}
# Here, the value referenced by variable "f" is converted to bool

bool(f)
```

::: {.output .execute_result execution_count="60"}
    False
:::
:::

::: {.cell .code execution_count="61"}
``` {.python}
g=-40
```
:::

::: {.cell .code execution_count="62"}
``` {.python}
# Here, the value referenced by variable "g" is converted to bool

bool(g)
```

::: {.output .execute_result execution_count="62"}
    True
:::
:::

::: {.cell .code}
``` {.python}
NOTE: In Numeric values, only 0 is insignificant, rest all numeric values are significant
```
:::

::: {.cell .markdown}
# 2) Float to other types of values {#2-float-to-other-types-of-values}
:::

::: {.cell .code execution_count="63"}
``` {.python}
a=30.2
```
:::

::: {.cell .code execution_count="64"}
``` {.python}
type(a)
```

::: {.output .execute_result execution_count="64"}
    float
:::
:::

::: {.cell .markdown}
`<b>`{=html}Conversion from float to integer: `</b>`{=html}`<br>`{=html}
1) Remove the decimal point as well as the digits that come after the
decimal point
:::

::: {.cell .code execution_count="65"}
``` {.python}
# Here, the value referenced by variable "a" is converted to integer

int(a)
```

::: {.output .execute_result execution_count="65"}
    30
:::
:::

::: {.cell .code execution_count="66"}
``` {.python}
b=30.9
```
:::

::: {.cell .code execution_count="67"}
``` {.python}
type(b)
```

::: {.output .execute_result execution_count="67"}
    float
:::
:::

::: {.cell .code execution_count="68"}
``` {.python}
# Here, the value referenced by variable "b" is converted to integer

int(b)
```

::: {.output .execute_result execution_count="68"}
    30
:::
:::

::: {.cell .code execution_count="69"}
``` {.python}
c=-40.987
```
:::

::: {.cell .code execution_count="70"}
``` {.python}
# Here, the value referenced by variable "c" is converted to integer

int(c)
```

::: {.output .execute_result execution_count="70"}
    -40
:::
:::

::: {.cell .markdown}
`<b>`{=html}Conversion to string:`</b>`{=html}`<br>`{=html} 1) Surround
the value with quotes(single quote)
:::

::: {.cell .code execution_count="71"}
``` {.python}
d=90.99
```
:::

::: {.cell .code execution_count="72"}
``` {.python}
type(d)
```

::: {.output .execute_result execution_count="72"}
    float
:::
:::

::: {.cell .code execution_count="73"}
``` {.python}
# Here, the value referenced by variable "d" is converted to string

str(d)
```

::: {.output .execute_result execution_count="73"}
    '90.99'
:::
:::

::: {.cell .code execution_count="74"}
``` {.python}
e=0.01
```
:::

::: {.cell .code execution_count="75"}
``` {.python}
type(e)
```

::: {.output .execute_result execution_count="75"}
    float
:::
:::

::: {.cell .code execution_count="76"}
``` {.python}
# Here, the value referenced by variable "e" is converted to boolean

bool(e)
```

::: {.output .execute_result execution_count="76"}
    True
:::
:::

::: {.cell .code execution_count="77"}
``` {.python}
f=0.00
```
:::

::: {.cell .code execution_count="78"}
``` {.python}
type(f)
```

::: {.output .execute_result execution_count="78"}
    float
:::
:::

::: {.cell .code execution_count="79"}
``` {.python}
# Here, the value referenced by variable "f" is converted to boolean

bool(f)
```

::: {.output .execute_result execution_count="79"}
    False
:::
:::

::: {.cell .code execution_count="80"}
``` {.python}
g=-30.9
```
:::

::: {.cell .code execution_count="81"}
``` {.python}
# Here, the value referenced by variable "g" is converted to boolean

bool(g)
```

::: {.output .execute_result execution_count="81"}
    True
:::
:::

::: {.cell .code execution_count="82"}
``` {.python}
q=12.87
```
:::

::: {.cell .code execution_count="83"}
``` {.python}
type(q)
```

::: {.output .execute_result execution_count="83"}
    float
:::
:::

::: {.cell .code}
``` {.python}
Conversion from float to integer:
1) Remove the decimal point as well as the digits that come after the decimal point
```
:::

::: {.cell .code execution_count="84"}
``` {.python}
# Here, the value referenced by variable "q" is converted to integer

int(q)
```

::: {.output .execute_result execution_count="84"}
    12
:::
:::

::: {.cell .code execution_count="85"}
``` {.python}
q
```

::: {.output .execute_result execution_count="85"}
    12.87
:::
:::

::: {.cell .markdown}
# 3) String to other types of values {#3-string-to-other-types-of-values}
:::

::: {.cell .code execution_count="86"}
``` {.python}
a="apple"
```
:::

::: {.cell .markdown}
`<b>`{=html}Inorder to convert string to integer, we need to follow the
below step:`</b>`{=html}`<br>`{=html} 1) Remove the quotes
:::

::: {.cell .code execution_count="87"}
``` {.python}
type(a)
```

::: {.output .execute_result execution_count="87"}
    str
:::
:::

::: {.cell .markdown}
`<b>`{=html}In the below code, we tried to convert a string value to
integer. For that we need to remove the quotes. However even after
removing the quotes, the resultant value was not a integer, hence python
returns a error.`</b>`{=html}
:::

::: {.cell .code execution_count="88"}
``` {.python}
int(a)
```

::: {.output .error ename="ValueError" evalue="invalid literal for int() with base 10: 'apple'"}
    ---------------------------------------------------------------------------
    ValueError                                Traceback (most recent call last)
    <ipython-input-88-8b2ab3991dae> in <module>
    ----> 1 int(a)

    ValueError: invalid literal for int() with base 10: 'apple'
:::
:::

::: {.cell .code execution_count="89"}
``` {.python}
b='50.9'
```
:::

::: {.cell .code execution_count="90"}
``` {.python}
type(b)
```

::: {.output .execute_result execution_count="90"}
    str
:::
:::

::: {.cell .markdown}
`<b>`{=html}In the below code, we tried to convert a string value to
integer. For that we need to remove the quotes. However even after
removing the quotes, the resultant value was not a integer, hence python
returns a error.`</b>`{=html}
:::

::: {.cell .code execution_count="91"}
``` {.python}
int(b)
```

::: {.output .error ename="ValueError" evalue="invalid literal for int() with base 10: '50.9'"}
    ---------------------------------------------------------------------------
    ValueError                                Traceback (most recent call last)
    <ipython-input-91-07ae29993d50> in <module>
    ----> 1 int(b)

    ValueError: invalid literal for int() with base 10: '50.9'
:::
:::

::: {.cell .code execution_count="92"}
``` {.python}
c='50'
```
:::

::: {.cell .code execution_count="93"}
``` {.python}
type(c)
```

::: {.output .execute_result execution_count="93"}
    str
:::
:::

::: {.cell .markdown}
`<b>`{=html}Inorder to convert string to integer, follow the below
step:`</b>`{=html}`<br>`{=html} 1) Remove the quotes
:::

::: {.cell .code execution_count="94"}
``` {.python}
# Here, the value referenced by variable "c" is converted to integer

int(c)
```

::: {.output .execute_result execution_count="94"}
    50
:::
:::

::: {.cell .markdown}
`<b>`{=html}Conversion from string to float:`</b>`{=html}`<br>`{=html}
1) Convert the value to a real number (remove the quotes) `<br>`{=html}
2) Convert the real number to a number with decimal `<br>`{=html}
:::

::: {.cell .code execution_count="95"}
``` {.python}
d='apple'
```
:::

::: {.cell .code execution_count="96"}
``` {.python}
type(d)
```

::: {.output .execute_result execution_count="96"}
    str
:::
:::

::: {.cell .markdown}
`<b>`{=html}In the below code, we tried to convert a string value to
float. For that we followed the two steps. However even after following
the two steps, the resultant value was not a float, hence python returns
a error.`</b>`{=html}
:::

::: {.cell .code execution_count="97"}
``` {.python}
float(d)
```

::: {.output .error ename="ValueError" evalue="could not convert string to float: 'apple'"}
    ---------------------------------------------------------------------------
    ValueError                                Traceback (most recent call last)
    <ipython-input-97-375ddbb813ae> in <module>
    ----> 1 float(d)

    ValueError: could not convert string to float: 'apple'
:::
:::

::: {.cell .code execution_count="98"}
``` {.python}
e='30'
```
:::

::: {.cell .code execution_count="99"}
``` {.python}
type(e)
```

::: {.output .execute_result execution_count="99"}
    str
:::
:::

::: {.cell .code execution_count="100"}
``` {.python}
# Here, the value referenced by variable "e" is converted to float

float(e)
```

::: {.output .execute_result execution_count="100"}
    30.0
:::
:::

::: {.cell .code execution_count="101"}
``` {.python}
f='30.9'
```
:::

::: {.cell .code execution_count="102"}
``` {.python}
type(f)
```

::: {.output .execute_result execution_count="102"}
    str
:::
:::

::: {.cell .markdown}
`<b>`{=html}Conversion from string to float:`</b>`{=html}`<br>`{=html}
1) Convert the value to a real number (remove the quotes)`<br>`{=html}
2) Convert the real number to a number with decimal`<br>`{=html}
:::

::: {.cell .code execution_count="103"}
``` {.python}
float(f)
```

::: {.output .execute_result execution_count="103"}
    30.9
:::
:::

::: {.cell .code execution_count="104"}
``` {.python}
x='apple'
```
:::

::: {.cell .code execution_count="105"}
``` {.python}
type(x)
```

::: {.output .execute_result execution_count="105"}
    str
:::
:::

::: {.cell .code execution_count="106"}
``` {.python}
# Here, the value referenced by variable "x" is converted to bool

bool(x)
```

::: {.output .execute_result execution_count="106"}
    True
:::
:::

::: {.cell .code execution_count="107"}
``` {.python}
len(x)
```

::: {.output .execute_result execution_count="107"}
    5
:::
:::

::: {.cell .code execution_count="108"}
``` {.python}
y=' '
```
:::

::: {.cell .code execution_count="109"}
``` {.python}
type(y)
```

::: {.output .execute_result execution_count="109"}
    str
:::
:::

::: {.cell .code execution_count="110"}
``` {.python}
len(y)
```

::: {.output .execute_result execution_count="110"}
    1
:::
:::

::: {.cell .code execution_count="111"}
``` {.python}
# Here, the value referenced by variable "y" is converted to bool

bool(y)
```

::: {.output .execute_result execution_count="111"}
    True
:::
:::

::: {.cell .code execution_count="112"}
``` {.python}
z=''
```
:::

::: {.cell .code execution_count="113"}
``` {.python}
type(z)
```

::: {.output .execute_result execution_count="113"}
    str
:::
:::

::: {.cell .code execution_count="114"}
``` {.python}
len(z)
```

::: {.output .execute_result execution_count="114"}
    0
:::
:::

::: {.cell .code execution_count="115"}
``` {.python}
# Here, the value referenced by variable "z" is converted to bool

bool(z)
```

::: {.output .execute_result execution_count="115"}
    False
:::
:::

::: {.cell .markdown}
`<b>`{=html}NOTE:`</b>`{=html}`<br>`{=html}1) In Numeric values, only 0
is insignificant, rest all numeric values are significant `<br>`{=html}
2) In String, only empty string is insignificant, rest all string values
are significant `<br>`{=html}
:::

::: {.cell .markdown}
# 4) Boolean to other types of values {#4-boolean-to-other-types-of-values}
:::

::: {.cell .code execution_count="116"}
``` {.python}
a=True
```
:::

::: {.cell .code execution_count="117"}
``` {.python}
type(a)
```

::: {.output .execute_result execution_count="117"}
    bool
:::
:::

::: {.cell .code execution_count="118"}
``` {.python}
# Here, the value referenced by variable "a" is converted to integer


int(a)
```

::: {.output .execute_result execution_count="118"}
    1
:::
:::

::: {.cell .code execution_count="119"}
``` {.python}
a
```

::: {.output .execute_result execution_count="119"}
    True
:::
:::

::: {.cell .markdown}
`<b>`{=html}Inorder to convert a boolean value to a float value, you
have to follow the below steps:`<br>`{=html}`</b>`{=html} 1) Convert the
value to a real number `<br>`{=html} 2) Convert the real number to a
number with decimal
:::

::: {.cell .code execution_count="120"}
``` {.python}
# Here, the value referenced by variable "a" is converted to float


float(a)
```

::: {.output .execute_result execution_count="120"}
    1.0
:::
:::

::: {.cell .code execution_count="121"}
``` {.python}
a
```

::: {.output .execute_result execution_count="121"}
    True
:::
:::

::: {.cell .markdown}
`<b>`{=html}Inorder to convert a boolean value to a string value, you
have to follow the below step:`<br>`{=html}`</b>`{=html} 1) Surround the
value with quotes(single quote)`<br>`{=html}
:::

::: {.cell .code execution_count="122"}
``` {.python}
# Here, the value referenced by variable "a" is converted to string


str(a)
```

::: {.output .execute_result execution_count="122"}
    'True'
:::
:::

::: {.cell .code execution_count="123"}
``` {.python}
b=False
```
:::

::: {.cell .code execution_count="124"}
``` {.python}
type(b)
```

::: {.output .execute_result execution_count="124"}
    bool
:::
:::

::: {.cell .code execution_count="125"}
``` {.python}
# Here, the value referenced by variable "b" is converted to integer

int(b)
```

::: {.output .execute_result execution_count="125"}
    0
:::
:::

::: {.cell .code execution_count="126"}
``` {.python}
b
```

::: {.output .execute_result execution_count="126"}
    False
:::
:::

::: {.cell .code execution_count="127"}
``` {.python}
# Here, the value referenced by variable "b" is converted to float

float(b)
```

::: {.output .execute_result execution_count="127"}
    0.0
:::
:::

::: {.cell .code execution_count="128"}
``` {.python}
b
```

::: {.output .execute_result execution_count="128"}
    False
:::
:::

::: {.cell .code execution_count="129"}
``` {.python}
# Here, the value referenced by variable "b" is converted to string

str(b)
```

::: {.output .execute_result execution_count="129"}
    'False'
:::
:::

::: {.cell .code}
``` {.python}
```
:::
