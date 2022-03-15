---
layout: home
title: Task 2
#permalink: index.html # in case of we remove the index.md file, this doc will be the index page
---

<div class="row">
<div class="columnStmt" markdown="1">

## Description
------
-   For `word = "hello"` and `skeletons = ["h--l0", "--llo", "g-llo", "h--l"]`, the output should be solution(word, `skeletons) = ["h--lo","--ll0"]`

    **Explanation:**
    -   `"h--lo"` is a skeleton of `"hello"` because you CAN fill in missing letters as follows:
    
        -   a)  `h` =` h`
        -   b)  `-` -> `e`
        -   c)  `-` -> `e`
        -   d)  `l` = `l`
        -   e)  `o` = `o`
  
    -   `"--llo"` is a skeleton of `"hello"` because you CAN fill in missing letters as follows:
    
        -   a)  `-` -> `h`
        -   b)  `-` -> `e`        
        -   c)  `l` = `l`
        -   d)  `l` = `l`
        -   e)  `o` = `o`
    
    -   `"ge-lo"` is NOT a skeleton of `"hello"` because you CANNOT fill in missing letters to form the word `"hello"`:
    
        -   a)  `g` != `h`
        -   a)  `e` != `e`               
        -   c)  `-` -> `l`
        -   d)  `l` = `l`
        -   e)  `o` = `o`
    
    -   `"h--l"` is NOT a skeleton of `"hello"` because you CANNOT fill in missing letters to form the word `"hello"`:
    
        -   a)  `h` =` h`
        -   b)  `-` -> `e`               
        -   c)  `-` -> `l`
        -   d)  `l` = `l`
        -   e)  nothing to substitute for 0. (The length of "h--l" is NOT the same as the length of the given word ``"hello"``)
    
    **Explanation:**
    -   `duo` is a skeleton of `duo`, as they already match.

    -   `"d-t"` is NOT a skeleton of `"duo"` because you CANNOT fill in missing letters to form the word `"duo"`:
    
        -   a)  `d` = `d`
        -   a)  `-` -> `u`               
        -   c)  `t` != `o` (t cannot be replaced with 0)
    
    -   `duo` is a skeleton of `duo`, as they already match.

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