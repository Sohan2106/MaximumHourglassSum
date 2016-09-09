# MaximumHourglassSum
Print the largest (maximum) hourglass sum found in an array (6 x 6)

Sample Input

<pre>1 1 1 0 0 0	<br/>
0 1 0 0 0 0 <br/>
1 1 1 0 0 0<br/>
0 0 2 4 4 0<br/>
0 0 0 2 0 0<br/>
0 0 1 2 4 0<br/></pre>

Sample Output
19

Explanation:
Array contains the following hourglasses:

<pre>1 1 1   1 1 0   1 0 0   0 0 0 <br/>
  1       0       0       0<br/>
1 1 1   1 1 0   1 0 0   0 0 0<br/>

0 1 0   1 0 0   0 0 0   0 0 0<br/>
  1       1       0       0<br/>
0 0 2   0 2 4   2 4 4   4 4 0<br/>

1 1 1   1 1 0   1 0 0   0 0 0<br/>
  0       2       4       4<br/>
0 0 0   0 0 2   0 2 0   2 0 0<br/>

0 0 2   0 2 4   2 4 4   4 4 0<br/>
  0       0       2       0<br/>
0 0 1   0 1 2   1 2 4   2 4 0<br/></pre>

The hourglass with the maximum sum (19) is:

<pre>2 4 4<br/>
  2<br/>
1 2 4<br/>
</pre>
