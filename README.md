# Missing_Value_prediction
##This Peoject is taken from HackerRank challenge. The question is the following
Objective
In this challenge, we practice predicting values. Check out the Resources tab for some tips on approaching this problem.
<p1>
Task
Given a record containing the maximum and minimum monthly temperatures at a particular station. The record shows the temperature information for each month in a data range from  to ; however, some of the temperature values have been blanked out! Estimate and print the missing values.
</p1>
<p1>
Input Format
</p1>
<p1>
The first line contains an integer, , denoting the number of rows of data in the input file.
The second line contains the header for the tab-separated file; this line can be ignored, and is simply there to make the test case easier to read.
The  subsequent lines each describe the respective , , , and  data as a row of tab-separated values. In some of the rows, The  or  temperature field has been blanked out and replaced by: , , etc.
</p1>
<p1>

Constraints
</p1>
<p1>

Scoring
</p1>
<p1>

The score seen upon hitting  is the score against the sample test case (of  rows) only. It is normalized and will always lie between  and .
Upon hitting , the score seen is determined solely on the basis of the hidden test case.

Details on the Scoring Formula
</p1>
<p1>

We compute the average of the magnitude of difference between your predicted value and the actual recorded value for each of the missing terms. If this average exceeds  degrees, you will be assigned a score of zero.

For each of the values predicted by you (), we will compute an . The  is the difference of the predicted value () and the actual temperature at that location. Hence,


We will compute the average of all these error terms over all rows of data in the input file, and record it as 

Your score for this challenge will be 
Here, .
</p1>
<p1>

Output Format
<p1>
</p1>

Print each missing value on a new line.
<p1>
</p1>
<p1>
Sample Input
</p1>
<p1>
20
 </p1>
<p1>
<table style="width:100%">
  <tr>
<th>yyyy</th>    <th>month</th>   <th>tmax</th>    <th>tmin</th></tr>
<tr>
    <td>1908</td><td>    January</td><td> 5.0 </td><td>-1.4</td>
  </tr>
<tr>
    <td>1908</td><td>    February</td><td>    7.3</td><td> 1.9</td>
  </tr>
<tr>
    <td>1908</td><td>    Marc</td><td>h   6.2</td><td> 0.3</td>
  </tr>
<tr>
    <td>1908</td><td>    April</td><td>   Missing_1</td><td>   2.1</td>
  </tr>
<tr>
    <td>1908</td><td>    May</td><td> Missing_2 </td><td>  7.7</td>
  </tr>
<tr>
    <td>1908</td><td>    June</td><td>    17.7</td><td>    8.7</td>
  </tr>
<tr>
    <td>1908</td><td>    July</td><td>    Missing_3</td><td>   11.0</td>
  </tr>
</table>
The above test case is for explanatory purposes only, which is why we included only  lines.
The sample test case, which is run upon hitting , has  rows of data.
The hidden test case, which is used at the time of submission, has over  rows of data. The sample test case rows are a subset of it.
<p1>
Sample Output
</p1>
The four missing values (, , , and ) are:
<table style="width:100%">
<tr>
    <td>8.6</td>
  </tr>
<tr>
    <td>15.8</td>
  </tr>
<tr>
    <td>18.9</td>
  </tr>
<tr>
    <td>0.0    </td>
  </tr>
</table>
Your task is to predict values as close as possible to these.
