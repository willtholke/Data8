# Data 8: Foundations of Data Science

    University of California, Berkeley
    Instructors: David Wagner, Ani Adhikari
    daw@cs.berkeley.edu, adhikari@berkeley.edu
    Office Hours: 12:00 pm - 5 pm in 145 Moffitt
    http://data8.org/fa21/office-hours.html
    Lecture: Mon/Wed/Fri 10:00am-11:00am 
    https://berkeley.zoom.us/j/97862154992
    Author: Will Tholke

## Table of Contents

- [Data 8: Foundations of Data Science](#data-8-foundations-of-data-science)
  - [Table of Contents](#table-of-contents)
  - [Lecture 1, 08/25/21 (Wk1): Introduction](#lecture-1-082521-wk1-introduction)
    - [Important Dates](#important-dates)
  - [Lecture 2, 08/27/21 (Wk1): Cause and Effect](#lecture-2-082721-wk1-cause-and-effect)
    - [Chocolate & Heart Disease](#chocolate--heart-disease)
    - [Causality vs. Confounding](#causality-vs-confounding)
  - [Lecture 3, 08/30/21 (Wk2): Tables](#lecture-3-083021-wk2-tables)
    - [Integers, Names, & Functions in Python](#integers-names--functions-in-python)
    - [Tables](#tables)
      - [Table Operations](#table-operations)
  - [Lecture 4, 09/01/21 (Wk2): Data Types](#lecture-4-090121-wk2-data-types)
    - [Ints and Floats](#ints-and-floats)
    - [Text, Strings, and Conversions](#text-strings-and-conversions)
    - [Discussion Question](#discussion-question)
    - [Types](#types)
    - [Arrays](#arrays)
  - [Lecture 5, 09/03/21 (Wk2): Building Tables](#lecture-5-090321-wk2-building-tables)
    - [Arrays (Continued)](#arrays-continued)
    - [Ranges](#ranges)
    - [Ways to Create a Table](#ways-to-create-a-table)
  - [Lecture 6, 09/08/21 (Wk3): Census](#lecture-6-090821-wk3-census)
    - [Manipulating Rows](#manipulating-rows)
    - [The Decennial Census](#the-decennial-census)
    - [The Census Table](#the-census-table)
  - [Lecture 7, 09/10/21 (Wk3): Charts](#lecture-7-091021-wk3-charts)
    - [Line vs. Scatter Plot](#line-vs-scatter-plot)
    - [Good Practices of Data Visualization](#good-practices-of-data-visualization)
    - [Statistical Data Types](#statistical-data-types)
  - [Lecture 8, 09/13/21 (Wk4): Histograms](#lecture-8-091321-wk4-histograms)
    - [Distributions: Terminology](#distributions-terminology)
    - [Bar Chart](#bar-chart)
    - [The `group` Method: Introduction](#the-group-method-introduction)
    - [Distributions of Quantitative Variables](#distributions-of-quantitative-variables)
    - [Area Principle](#area-principle)
    - [Histograms](#histograms)
    - [Calculating Height](#calculating-height)
    - [Calculating Areas](#calculating-areas)
    - [Finalé: Bar Chart or Histogram?](#finalé-bar-chart-or-histogram)
  - [Lecture 9, 09/15/21 (Wk4): Functions](#lecture-9-091521-wk4-functions)
    - [Review: Area vs. Height](#review-area-vs-height)
    - [Defining Functions](#defining-functions)
    - [Apply](#apply)
  - [Lecture 10, 09/17/21 (Wk4): Groups](#lecture-10-091721-wk4-groups)
    - [Grouping](#grouping)
    - [Lists](#lists)
    - [Grouping by Multiple Columns](#grouping-by-multiple-columns)
    - [Pivot](#pivot)
    - [Group or Pivot?](#group-or-pivot)
  - [Lecture 11, 09/20/21 (Wk5): Joins](#lecture-11-092021-wk5-joins)
    - [Create a Full Table with Lists](#create-a-full-table-with-lists)
    - [What about list -> array conversion?](#what-about-list---array-conversion)
  - [Lecture 12, 09/22/21 (Wk5): Table Examples](#lecture-12-092221-wk5-table-examples)
    - [Important Table Methods](#important-table-methods)
  - [Lecture 13, 09/24/21 (Wk5): Conditionals & Iteration](#lecture-13-092421-wk5-conditionals--iteration)
    - [Comparison Operators](#comparison-operators)
    - [Control Statements](#control-statements)
    - [Random](#random)
- [A Longer Array](#a-longer-array)
- [`for` Statements](#for-statements)
- [Advanced `where`](#advanced-where)
  - [Lecture 14, 09/27/21 (Wk6): Chance](#lecture-14-092721-wk6-chance)
    - [Subtitle #1](#subtitle-1)
  - [Lecture 15, 09/29/21 (Wk6): Sampling](#lecture-15-092921-wk6-sampling)
    - [Subtitle #1](#subtitle-1-1)
  - [Lecture 16, 10/01/21 (Wk6): Models](#lecture-16-100121-wk6-models)
    - [Subtitle #1](#subtitle-1-2)
  - [Lecture 17, 10/04/21 (Wk7): Comparing Distributions](#lecture-17-100421-wk7-comparing-distributions)
    - [Subtitle #1](#subtitle-1-3)
  - [Lecture 18, 10/06/21 (Wk7): Decisions and Uncertainty](#lecture-18-100621-wk7-decisions-and-uncertainty)
    - [Subtitle #1](#subtitle-1-4)
  - [Lecture 19, 10/08/21 (Wk7): A/B Testing](#lecture-19-100821-wk7-ab-testing)
    - [Subtitle #1](#subtitle-1-5)
  - [Lecture 20, 10/11/21 (Wk8): Causality](#lecture-20-101121-wk8-causality)
    - [Subtitle #1](#subtitle-1-6)
  - [Lecture 21, 10/13/21 (Wk8): Examples](#lecture-21-101321-wk8-examples)
    - [Subtitle #1](#subtitle-1-7)
  - [Lecture 22, 10/03/21 (Wk8): Midterm Review](#lecture-22-100321-wk8-midterm-review)
    - [Subtitle #1](#subtitle-1-8)
  - [Lecture 23, 10/18/21 (Wk9): Confidence Intervals](#lecture-23-101821-wk9-confidence-intervals)
    - [Subtitle #1](#subtitle-1-9)
  - [Lecture 24, 10/20/21 (Wk9): Interpreting Confidence](#lecture-24-102021-wk9-interpreting-confidence)
    - [Subtitle #1](#subtitle-1-10)
  - [Lecture 25, 10/22/21 (Wk9): Center and Spread](#lecture-25-102221-wk9-center-and-spread)
    - [Subtitle #1](#subtitle-1-11)
  - [Lecture 26, 10/25/21 (Wk10): The Normal Distribution](#lecture-26-102521-wk10-the-normal-distribution)
    - [Subtitle #1](#subtitle-1-12)
  - [Lecture 27, 10/27/21 (Wk10): Sample Means](#lecture-27-102721-wk10-sample-means)
    - [Subtitle #1](#subtitle-1-13)
  - [Lecture 28, 10/29/21 (Wk10): Designing Experiments](#lecture-28-102921-wk10-designing-experiments)
    - [Subtitle #1](#subtitle-1-14)
  - [Lecture 29, 11/01/21 (Wk11): Correlation](#lecture-29-110121-wk11-correlation)
    - [Subtitle #1](#subtitle-1-15)
  - [Lecture 30, 11/03/21 (Wk11): Linear Regression (and it's my birthday!)](#lecture-30-110321-wk11-linear-regression-and-its-my-birthday)
    - [Subtitle #1](#subtitle-1-16)
  - [Lecture 31, 11/05/21 (Wk11): Least Squares](#lecture-31-110521-wk11-least-squares)
    - [Subtitle #1](#subtitle-1-17)
  - [Lecture 32, 11/08/21 (Wk12): Residuals](#lecture-32-110821-wk12-residuals)
    - [Subtitle #1](#subtitle-1-18)
  - [Lecture 33, 11/10/21 (Wk12): Regression Inference](#lecture-33-111021-wk12-regression-inference)
    - [Subtitle #1](#subtitle-1-19)
  - [Lecture 34, 11/12/21 (Wk12): Privacy](#lecture-34-111221-wk12-privacy)
    - [Subtitle #1](#subtitle-1-20)
  - [Lecture 35, 11/15/21 (Wk13): Classification](#lecture-35-111521-wk13-classification)
    - [Subtitle #1](#subtitle-1-21)
  - [Lecture 36, 11/17/21 (Wk13): Classifiers](#lecture-36-111721-wk13-classifiers)
    - [Subtitle #1](#subtitle-1-22)
  - [Lecture 37, 11/19/21 (Wk13): Decisions](#lecture-37-111921-wk13-decisions)
    - [Subtitle #1](#subtitle-1-23)
  - [Lecture 38, 11/22/21 (Wk14): TBA](#lecture-38-112221-wk14-tba)
    - [Subtitle #1](#subtitle-1-24)
  - [Lecture 39, 11/29/21 (Wk15): TBA](#lecture-39-112921-wk15-tba)
    - [Subtitle #1](#subtitle-1-25)
  - [Lecture 40, 12/03/21 (Wk15): Conclusion](#lecture-40-120321-wk15-conclusion)
    - [Subtitle #1](#subtitle-1-26)


## Lecture 1, 08/25/21 (Wk1): Introduction

### Important Dates

- **Midterm:** Friday October 15, 7-9pm PT
- **Final:** Monday, December 13, 8-11am PT
- **Labs:** due Wednesdays, 9am
- **Homework:** due Thursdays, 12am

## Lecture 2, 08/27/21 (Wk1): Cause and Effect

### Chocolate & Heart Disease

**Question:** Is there any relation between chocolate consumption and heart disease?
- Individuals, study subjects, participants, units: 336,289 US, Swedish, & Australian adults in various studies
- Treatment: chocolate consumption
- Outcome: heart disease

**Answer:** Yes, because those who ate chocolate had less heart disease

### Causality vs. Confounding

If the **treatment** and **control** groups are similar apart from the treatment, then differences between the outcomes in the two groups can be ascribed to the treatment (causality).

However, if the **treatment** and **control** groups have systematic differences other than the treatment, then it might be difficult to identify causality (due to counfounding variables).

Therefore, **randomized controlled experiments** are considered to be the industry standard.

## Lecture 3, 08/30/21 (Wk2): Tables

Check out the [Data8 Python Reference](http://data8.org/sp19/python-reference.html) for more comprehensive documentation

### Integers, Names, & Functions in Python

```py
# Integers
>>> 2 ** 4  # 2^4
16
>>> 2 + 8
10
>>> 5.0 + 2 * 9  # 5.0 + (2 * 9)
23.0

# Names
>>> a = 1
>>> b = 2
>>> total = a + b
>>> total
3

# Functions & Call Expressions
>>> abs(-5)
5
>>> round(123.456)
123
>>> round(123.456, ndigits=2)
123.46
```

### Tables

- A `Table` is a sequence of labeled columns
- Each **row** represents one individual
- Data within a **column** represents one attribute of the individuals

#### Table Operations

- `t.select(label)` - constructs a new table with just the specified columns
- `t.drop(label)` - constructs a new table in which the specified columns are omitted
- `t.sort(label)` - constructs a new table with rows sorted by the specified column
- `t.where(label, condition)` - constructs a new table with the rows that meet the condition


## Lecture 4, 09/01/21 (Wk2): Data Types

### Ints and Floats

**Python has two real number types:**

- **int:** integer of any size
  - never has a decimal point, e.g. `2` or `3`
- **float:** a number with an optional fraction part
  - always has a decimal point, e.g. `2.0` or `3.14`
  - s**ome limitations:** limited precision of 15-16 decimal places, arithmetic may result in the final few decimal places being wrong, have limited size

### Text, Strings, and Conversions

A string value is a snippet of text of any length

- `'a'`, `'word'`, `"there can be 2 sentences. Here's the second!"`
- Type conversions: `int('12')` becomes `12`, `float('1.2')` becomes `1.2`, or `str(5)` becomes `"5"`
  - `int(1.2)` becomes `1.0`, effectively **losing** information! Beware of this!

### Discussion Question

**Assume you have run the following statements:**

```py
>>> x = 3
>>> y = '4'
>>> z = '5.6'
```

What is the source of error in each example?

- **A.** `x + y`
  - You cannot add an int with a string
- **B.** `x + int(y + z)`
  - `int(y + z)` will throw an error; y + z is '45.6', but int('45.6') will not work
- **C.** `str(x) + int(y)`
  - You cannot add a string with an int
- **D.** `y + float(z)`
  - You cannot add a string with a float

### Types

We've seen the following types so far:

- **int:** `2`
- **float:** `2.2`
- **str:** `'Hello there!'`
- **builtin_function_or_method:** `abs()`
- **Table**

The `type()` function can tell you the type of a value

### Arrays

**An array contains a sequence of values:**

- All elements of an array should have the **same type**
- Arithmetic is applied to each individual element
- Adding arrays together adds elements (if same length!)
- A column of a table is an array

## Lecture 5, 09/03/21 (Wk2): Building Tables

### Arrays (Continued)

```py
>>> my_array = make_array(1, 2, 3, 4)  # assign array object to my_array
>>> my_array
array([1, 2, 3, 4])
>>> len(my_array)  # returns the num items in an array
4
>>> sum(my_array)
10
>>> np.average(my_array)
2.5
>>> array_2 = make_array(70, 60, 90, 80)
>>> array_2
array([70, 60, 90, 80])
>>> my_array + array_2  # arrays msut be the same length to add
array([71, 62, 93, 84])
>>> array_3 = make_array(5, 6, 7)
>>> array_3 + array _2
ValueError: operands could not be broadcast together with shapes (4,) (3,)
>>> array_3.item(0)
5
```

### Ranges

A range is an array of consecutive numbers:

- The range always includes start but excludes end
- `np.arange(end)`: an array of increasing integers from 0 up to end
- `np.arange(start, end)`: an array of increasing integers from start up to end
- `np.arange(start, end, step)`: a range with `step` between consecutive values

### Ways to Create a Table

- `Table.read_table(filename)` reads a table from .csv
- `Table()` creates an empty table
- `select, where, sort` etc. is also useful

```py
>>> streets = make_array('Bancroft', 'Durant', 'Channing', 'Haste')
>>> streets
array(['Bancroft', 'Durant', 'Channing', 'Haste'], dtype='<U8')
>>> Table()
# no output
>>> southside = Table().with_column('Streets', streets)
>>> southside
  ________
| streets  |
  ________
| Bancroft |
  ________
| Durant   |
  ________
| Channing |
  ________
| Haste    |
  ________
```

## Lecture 6, 09/08/21 (Wk3): Census

### Manipulating Rows
  
- `t.sort(column)`: sorts the rows in increasing order
- `t.sort(column, descending=True)`: sorts the rows in decreasing order
- `t.take(row_numbers)`: keeps the numbered rows
- `t.where(column, are.conditions)`: keeps the rows for which a column's value satisfies a condition
- `t.where(column, are.equal_to(value))` keeps rows for whcih a column's value equals a particular value

### The Decennial Census

- Every ten years, the Census Bureau counts how many people there are in the United States
- In between censues, the Bureau makes an estimate about how many people there are each year
  
### The Census Table

- Values have column-dependent interpretations
  - The `SEX` column: 1 is `Male`, 2 is `Female`
  - The `POPESTIMATE2010` column: 7/1/2010 estimate
- Some rows are the sum of other rows
  - The `SEX` column: 0 is total of `Male` and `Female` categories
  - The `AGE` column: 999 is the total of all ages
- Numeric codes are used for storage efficiency


## Lecture 7, 09/10/21 (Wk3): Charts

### Line vs. Scatter Plot

- `t.plot(x_label, y_label)`
  - Use for sequential quantitative data iff 
    - x-axis has order
    - sequential differences in y are meaningful
    - 1:1 ratio of y-value to x-value
    - **oftentimes,** x-axis is *time* and y-axis is *distance*
- `t.scatter(x_label, y_label)`
  - Use for non-sequential quantitative data

### Good Practices of Data Visualization
  
- **Less can be more!**
  - Minimize decoration
  - Minimize colors
- **Represent numerical data correctly**; i.e. preserve their relative values and distances between one another

### Statistical Data Types

- **Quantitative:** measured numerically (age, population size)
- **Categorical:** 
  - Unordered (color of shoes)
  - Ordered ("not satisfied, satisfied, very satisfied")

- **"Numerical"** *(but actually categorical)* **variables**:
  - 1 for "Berkeley student", 0 for "not a Berkeley student
  - Doing arithmetic with the numbers is arbitrary and useless
  - Distances between numerical values have no clear meaning

## Lecture 8, 09/13/21 (Wk4): Histograms

### Distributions: Terminology

- **Individuals:** those whose features are recorded
- **Variable:** a feature, an attribute
  - can be *quantitative* or *categorical* (and of many sub-types within these)
  - has different values
  - each *individual* has exactly *one value*
  - has a *distribution:*
    - for each different value of the variable, the frequency of individuals that have that value

In a distribution, each individual is ine exactly one category. The sum of the percent of individuals in each category adds up to 100%.

### Bar Chart

- **Utility:** display all the values of the variables along with their frequencies; the attributes are as folows:
  - one bar for each category
  - you can choose the order of the bars
  - length of the bar is the percent (or count) of individuals in that category
  
### The `group` Method: Introduction

- The `group` method counts the number of rows for each value in the column

**Example:**

```py
studios = top_movies.select('Studio')
studios.group('Studio').show(3)
```

### Distributions of Quantitative Variables

- Binning is counting the number of numerical values that lie within ranges, called *bins*:
  - Bins are defined by their lower bounds (inclusive)
  - The upper bound (exclusive) is the lower bound of the next bin

### Area Principle

**Areas** should be proportional to the values they represent;
- 20% of a population can be represented by (x)
- 40% of a population cab be represented by (x)(x), but not by a large (X)

### Histograms

- **Utility:** display the distribution of a quantitative variable
  - One bar corresponds to each bin
  - Uses the area principle
    - The *area* of each bar is the *percent* of individuals in the corresponding bin

- You can create a histogram by using `hist`, which uses a scale `(normed=True)` that ensures the area of the chart sums to 100%
- The *area* of each bar is a percentage of the whole
  - The whole sums to 100%
- The horizontal axis is a number line (e.g. years) and the bins sizes don't have to be equal to each other
- The gvertical axis is a rate (e.g., percent per year)
  
### Calculating Height

The [40, 60) bin contains 46 out of 200 movies
- "46 out of 200" is 23% of the whole
- The bin is 60 - 40 = 20 years wide

```
Height of bar = 23 percent / 20 years 
              = 1.15 percent per year
```

```
Height of bar = % of the whole in bin / width of bin
              = ## percent per unit of width
```

- The height measures the percent of data in the bin *relative to the amount of space in the bin.*
- Height measures **density** (crowdedness)
- Units: percept per unit on the horizontal axis

### Calculating Areas

```
Area of bar = % in bin 
            = height x width of bin
```

**Question:** how many individuals are in the bin?

- **Answer:** use area

**Question:** how crowded is the bin?

- **Answer:** use height

### Finalé: Bar Chart or Histogram?

**Use a bar chart when:**

- Distribution of categorical variable
- Bars have arbitrary (but equal) widths and spacings; in any order
- height (or length) and area of bars proportional to the percent of individuals
  
**Use a histogram when:**

- Distribution of quantitative variable
- Horizontal axis is numerical; drawn to scale, no gaps, bins can be unequal
- Area of bars proportional to the percent of individuals; height measures density

## Lecture 9, 09/15/21 (Wk4): Functions

### Review: Area vs. Height
  
```
Area of Bar = Percent in Bin
            = Height x Bin Width
```

How many individuals... use *area*; how crowded(dense)... use *height*

### Defining Functions

The following block of code is a function in Python

```py
def spread(values):
  return max(values) - min(values)
```

The `spread()` function contains the following:

- **Name:** `spread`
- **Argument names (parameters):** `values`
- **Body:** `return max(values) - min(values)`
- **Return expression:** ` max(values) - min(values)`

### Apply

What does apply do?

- It calls a function on every element in the input column(s)
- Returns an array that contains the function applied to every element
  - `table_name.apply(funciton_name, 'column_label(s)')`
- `function_name` refers to the function that is to be applied to the specified input columns `column_label(s)`


## Lecture 10, 09/17/21 (Wk4): Groups

### Grouping

The `group` method aggregates all rows with the same value for a column into a single row in the resulting table

- First argument: which column to group by
- Second argument: (Optional) how to combine values
  - len – number of grouped values (default)
  - list – list of all grouped values
  - sum – total of all grouped values

### Lists

A list is a sequence of values (just like an array), but the values can have different types:

- Lists can be used to create table rows
- If you create a table column from a list, it will be converted to an array automatiaclly

### Grouping by Multiple Columns

The `group` method can also aggregate all rows that share the combination of values in multiple columns
- **First argument:** a list of which columns to group by
- `collect=...`: (Optional) how to combine values

### Pivot

- Cross-classifies according to two categorial variables
- Produces a grid of counts or aggregated values
- Two required arguments:
  - First: variable that forms column labels of grid
  - Second: variable that forms row labels of grid
- Two optional arguments (include both or neither):
  - `values='column_label_to_aggregate`
  - `collect=function_to_aggregate_with`

```py
# Out of context example
sky.pivot('city', 'material', values='height', collect=max)
```

### Group or Pivot?

- Distribution of one categorical variable -> `.group()`
- Cross classification of two or more categorical variables:
  - One row per combination -> `.group()`
  - One variable vertically, one horizontally -> `.pivot()`


## Lecture 11, 09/20/21 (Wk5): Joins

### Create a Full Table with Lists

```py
>>> drinks = Table(['Drink', 'Cafe', 'Price])
>>> drinks # this will show the table on the next line
Drink | Cafe | Price |
----------------------
```

```py
>>> drinks = drinks.with_rows([["Milk Tea", "Feng Cha", 5.5], ...]]) # nested list
>>> drinks
Drink    |   Cafe   | Price |
-----------------------------
Milk Tea | Feng Cha |  5.5  |
...
```

### What about list -> array conversion?

You can only convert a list to an array when all of the elements in the list are of the same type!

- **Valid:** `[1, 2, 3, 4, 5]`
- **Invalid:** `[1, 2, 3, 4, "dog"]` (all integers will be converted to strings; you don't want this)


## Lecture 12, 09/22/21 (Wk5): Table Examples

### Important Table Methods
  
```py
>>> t.select(column, …) or t.drop(column, …)
>>> t.take([row_num, …]) or t.exclude([row_num, …])
>>> t.sort(column, descending=False)
>>> t.where(column, are.condition(...)) 
>>> t.apply(function_name, column, …)
>>> t.group(column) or t.group(column, function_name)
>>> t.group([column, …]) or t.group([column, …], function_name)
>>> t.pivot(cols, rows) or t.pivot(cols, rows, vals, function_name)
>>> t.join(column, other_table, other_table_column)
```

## Lecture 13, 09/24/21 (Wk5): Conditionals & Iteration

### Comparison Operators

Note that the result of a comparison expression is a `bool` value, named after [George Boole](https://en.wikipedia.org/wiki/George_Boole)


```py
# Assignment Statement
>>> x = 2
>>> y = 3

# Comparison Expression
>>> x > 1
True
>>> x > 100
False
>>> x == y
False
>>> 2 < x < 5
False
>>> 1 + 1 + 0 == 2
True
```

### Control Statements

These statements *control* the sequence of computations that are performed in a program

- The keywords `if` and `for` begin control statemnets
- The purpose of an `if` statement is to define functions that choose different behavior based on their arguments
  

### Random

`np.random.choice`:

- Selects uniformly at random
- with replacement
- from an array
- a specified number of times
  - e.x.: `np.random.choice(some_array, sample_size)`

# A Longer Array

`np.append(array_1, value)`

- new array with `value` appended to `array_1`
- `value` has to be of the same type of elements as `array_1`

# `for` Statements

- `for` is a keyword that beings a control statement
  - You can think about `for` as "for item in iterable"
- `for` performs a computation for every element in a list or array
  
```py
for item in some_array:
  print(item)
```

# Advanced `where`

`t.where(array_of_bool_values)`

- returns a table with only the rows of t for which the corresponding `bool` is True


## Lecture 14, 09/27/21 (Wk6): Chance

### Subtitle #1
  
-

## Lecture 15, 09/29/21 (Wk6): Sampling

### Subtitle #1
  
-

## Lecture 16, 10/01/21 (Wk6): Models

### Subtitle #1
  
-

## Lecture 17, 10/04/21 (Wk7): Comparing Distributions

### Subtitle #1
  
-

## Lecture 18, 10/06/21 (Wk7): Decisions and Uncertainty

### Subtitle #1
  
-

## Lecture 19, 10/08/21 (Wk7): A/B Testing

### Subtitle #1
  
-

## Lecture 20, 10/11/21 (Wk8): Causality

### Subtitle #1
  
-

## Lecture 21, 10/13/21 (Wk8): Examples

### Subtitle #1
  
-

## Lecture 22, 10/03/21 (Wk8): Midterm Review

### Subtitle #1
  
-

## Lecture 23, 10/18/21 (Wk9): Confidence Intervals

### Subtitle #1
  
-e

## Lecture 24, 10/20/21 (Wk9): Interpreting Confidence

### Subtitle #1
  
-e

## Lecture 25, 10/22/21 (Wk9): Center and Spread

### Subtitle #1
  
-e

## Lecture 26, 10/25/21 (Wk10): The Normal Distribution

### Subtitle #1
  
-e

## Lecture 27, 10/27/21 (Wk10): Sample Means

### Subtitle #1
  
-e

## Lecture 28, 10/29/21 (Wk10): Designing Experiments

### Subtitle #1
  
-e

## Lecture 29, 11/01/21 (Wk11): Correlation

### Subtitle #1
  
-

## Lecture 30, 11/03/21 (Wk11): Linear Regression (and it's my birthday!)

### Subtitle #1
  
-

## Lecture 31, 11/05/21 (Wk11): Least Squares

### Subtitle #1
  
-

## Lecture 32, 11/08/21 (Wk12): Residuals

### Subtitle #1
  
-

## Lecture 33, 11/10/21 (Wk12): Regression Inference

### Subtitle #1
  
-

## Lecture 34, 11/12/21 (Wk12): Privacy

### Subtitle #1
  
-

## Lecture 35, 11/15/21 (Wk13): Classification

### Subtitle #1
  
-

## Lecture 36, 11/17/21 (Wk13): Classifiers

### Subtitle #1
  
-

## Lecture 37, 11/19/21 (Wk13): Decisions

### Subtitle #1
  
-

## Lecture 38, 11/22/21 (Wk14): TBA

### Subtitle #1
  
-

## Lecture 39, 11/29/21 (Wk15): TBA

### Subtitle #1
  
-

## Lecture 40, 12/03/21 (Wk15): Conclusion

### Subtitle #1
  
*Note:* Final exam on Monday, 12/13/21 @ 8:00am-11:00am
-
