Download Link: https://assignmentchef.com/product/solved-comp1020-lab11-simple-sorting-the-selection-sort
<br>
<ul>

 <li>Simple sorting – the Selection Sort</li>

</ul>

Notes:

<ul>

 <li>The three exercises in this lab are independent – they can be done in any order. However, the Gold exercise is very similar to the Bronze exercise, and it would be best to do the Bronze exercise first.</li>

 <li>Only one of the three exercises is required, but try to do as many as you can.</li>

</ul>

Selection Sort to print an ArrayList

<ol>

 <li>Start with the file <strong>java</strong>.</li>

 <li>Complete the <strong>printInOrder</strong> method at the end of the file. This method will accept an <strong>ArrayList&lt;Integer&gt; data</strong> as its parameter. It will <em>not</em> sort this list. Instead, it will use a modified selection sort algorithm to simply <em>print</em> the list in ascending order. The list should be printed on a single line. As each number is printed, it can be deleted from <strong><sub>data</sub></strong>, so that when the method is finished, the list <strong><sub>data</sub></strong> will be an empty list.</li>

 <li>The output from the program should look like this. (The data will be random.)</li>

</ol>

<strong>Original list:  </strong>

<strong>[27, 44, 22, 20, 41, 29, 10, 2, 33, 7, 16, 26, 13, 44, 15, 15, 23, 11, 42, 13] </strong>

<strong>Print the list in ascending order: </strong>

<strong>2 7 10 11 13 13 15 15 16 20 22 23 26 27 29 33 41 42 44 44  </strong>

<strong>Original list (should be empty):  </strong>

<strong>[]</strong>




<ol>

 <li>Start with the files <strong>java</strong>, <strong>IntLL-template.java</strong>, and <strong>Node.java</strong>. Immediately rename the second file <strong>IntLL.java</strong>. This file implements a linked list of <strong>int</strong> data. A constructor and a few other suitable methods are already defined for you.</li>

 <li>Complete the <strong>void selSort()</strong> method in the <strong>IntLL</strong> class, so that it will perform a selection sort algorithm to re-arrange the <strong><sub>Node</sub></strong>s in the linked list so that the data is in ascending order.</li>

 <li>Half of the algorithm has been done for you – the <strong>Node largestPrev()</strong> method will find the <strong>Node</strong> in the list that contains the largest data item. (Since it’s easiest to add new nodes to the front of a linked list, you need the largest one each time, not the smallest one, if you want to get it into ascending order.) It will not return a reference to that <strong><sub>Node</sub></strong> – it will return a reference to the <em>previous</em> <strong><sub>Node</sub></strong>, since that is what you will need to remove it from the original unsorted list.</li>

 <li>You should not create any new nodes at all. The existing nodes must be re-linked into a new order, but nothing should be created or destroyed.</li>

 <li>When you run <strong>TestLab11Silver</strong>, the output should be as shown below. (The data is random.)</li>

</ol>

<strong>Original list:  </strong>

<strong>&lt;&lt; 41  34  29  40  30  33  17  16  30  16  37  49  3  8  34  28  49  38  7  44 &gt;&gt; </strong>

<strong>Sorted list:  </strong>

<strong>&lt;&lt; 3  7  8  16  16  17  28  29  30  30  33  34  34  37  38  40  41  44  49  49 &gt;&gt; </strong>

Non-destructive version of the Bronze exercise

<ol>

 <li>Begin with the file <strong>java</strong>.</li>

 <li>This is exactly the same as the Bronze exercise: Complete the <strong>printInOrder</strong> method at the end of the file. This method will accept an <strong>ArrayList&lt;Integer&gt; data</strong> as its parameter. It will <em>not</em> sort this list. Instead, it will use a modified selection sort algorithm to simply <em>print</em> the list in ascending order. The list should be printed on a single line.</li>

 <li>Here’s the tricky part. This time, the list <em>may not</em> be changed at any time. You must leave the original list <strong>data</strong> completely untouched (you can use <strong>.get()</strong> and <strong>.size()</strong> but nothing else). You also must not use any other array or list of any type (no arrays, no linked lists, no <strong>ArrayList</strong>s – nothing but simple <strong>int</strong> variables). Good luck.</li>

 <li>The output from the program should look like this. (The data will be random – there might be duplicate values in the list.)</li>

</ol>

<strong>Original list:  </strong>

<strong>[29, 8, 25, 19, 3, 23, 38, 15, 36, 19, 4, 14, 3, 20, 23, 10, 4, 8, 27, 41] </strong>

<strong>Print the list in ascending order: </strong>

<strong>3 3 4 4 8 8 10 14 15 19 19 20 23 23 25 27 29 36 38 41  </strong>

<strong>Original list (should be unchanged):  </strong>

<strong>[29, 8, 25, 19, 3, 23, 38, 15, 36, 19, 4, 14, 3, 20, 23, 10, 4, 8, 27, 41] </strong>


