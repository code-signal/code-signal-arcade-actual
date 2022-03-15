---
layout: home
title: Task 1
#permalink: index.html # in case of we remove the index.md file, this doc will be the index page
---

<div class="row">
<div class="columnStmt" markdown="1">

## Description
------
Given an array of non-negative integers a, your task is to test all the consecutive triples of elements for being a Pythagorean. In other words, for each triple of consecutive elements (a[i], a[i+1], a[i+2]) check whether the sum of squares of two of them equals the square of the remaining one, i.e. whether any of the following equations is true:

-   ![math_1_4_1](./img/math_1_4_1.png)

Return an array of length a.length -2, where the ith element is 1 if (a[i], a[i+1], a[i+2]) is a Pythagorean triple and 0 otherwise.

**Example**

For` a = [0, 5, 5, 0, 5, 13, 12]`, the output should be `solution(a) = [1, 1, 1, 0, 1]`.

-   Triple `(a[0], a[1], a[2]) = (0, 5, 5)` **is** a *Pythagorean triple*, because `a[0]^2 + a[1]^2 = a[2]^2`;
-   Triple `(a[1], a[2], a[3]) = (5, 5, 0)` **is** a *Pythagorean triple*, because `a[1]^2 + a[3]^2 = a[2]^2`;
-   Triple `(a[2], a[3], a[4]) = (5, 0, 5)` **is** a *Pythagorean triple*, because `a[2]^2 + a[3]^2 = a[4]^2`;
-   Triple `(a[3], a[4], a[5]) = (0, 5, 13)` **is Not** a *Pythagorean triple*, because none of the needed equations are true;
-   Triple `(a[4], a[5], a[6]) = (5, 13, 12)` **is** a *Pythagorean triple*, because `a[4]^2 + a[6]^2 = a[5]^2`;

**Input/Output**

* **[execution time limit] 4 seconds (js)**

* **[input] array.integer sequence**

A 2-dimensional array of integers representing a rectangular matrix of the building.

*Guaranteed constraints*:

<code>1 ≤ matrix.length ≤ 5</code>,
<code>1 ≤ matrix[i].length ≤ 5</code>,
<code>0 ≤ matrix[i][j] ≤ 10</code>.

* **[output] integer**

The total price of all the rooms that are suitable for the CodeBots to live in.

**[JavaScript (ES6)] Syntax Tips**

{% highlight javascript linenos=table %}
// Prints help message to the console
// Returns a string
function helloWorld(name) {
    console.log("This prints to the console when you Run Tests");
    return "Hello, " + name;
}
{% endhighlight %}

</div>
<div class="columnSol" markdown="1">

## Solution
------

{% highlight javascript linenos=table %}

{% include_relative solution.js %}

{% endhighlight %}

</div>
</div>