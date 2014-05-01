---
layout: lesson
root: ../..
---

## Relational Databases


<div>
<h4 id="person">Person</h4>
<table>
    <tr>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>

</div>


<div class="objectives">
<h4 id="objectives">Objectives</h4>
<ul>
<li>Explain what a relational database is</li>
<li>Explain primary keys, foreign keys</li>
<li>Explain how a database has multiple tables and why they relate to each other</li>
</ul>
</div>

### Primary Key


<div>
<p>To make using our database easier, we can add a key field to our database. A key is a special field in a database where the values in the field can be used to identify records.</p>
</div>


<div>
<h4 id="person">Person</h4>
<table>
    <tr>
        <th>
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td>
<strong>dyer</strong>
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td>
<strong>pb</strong>
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td>
<strong>lake</strong>
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td>
<strong>roe</strong>
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td>
<strong>danforth</strong>
</td>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>

</div>


<div>
<p>Here, we've added an <strong><code>ident</code></strong> field where each record has a unique value. This type of key, where each record is uniquely identified, is called a <strong>Primary Key</strong>.</p>
</div>

### Adding Data to our Database


<div>
<h4 id="person">Person</h4>
<table>
    <tr>
        <th>
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td>
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td>
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td>
danforth
</td>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>

</div>


<div>
<p>So far, our database only contains <code>Person</code> information from the Pole of Inaccessibility expeditions. We need to bring in more data to do any useful analysis.</p>
</div>


<div>
<p>We can insert data from each of the readings taken on the expedition</p>
</div>


<div>
<table>
    <tr>
        <th>
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
        <th>
Quant
</th>
        <th>
Reading
</th>
    </tr>
    <tr>
        <td>
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
        <td>
rad
</td>
        <td>
7.8
</td>
    </tr>
    <tr>
        <td>
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
        <td>
rad
</td>
        <td>
9.82
</td>
    </tr>
    <tr>
        <td>
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
        <td>
sal
</td>
        <td>
0.09
</td>
    </tr>
    <tr>
        <td>
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
        <td>
sal
</td>
        <td>
0.13
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
        <td>
rad
</td>
        <td>
4.35
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
        <td>
rad
</td>
        <td>
7.22
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
        <td>
rad
</td>
        <td>
8.41
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
        <td>
temp
</td>
        <td>
-21.5
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
        <td>
temp
</td>
        <td>
-18.5
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
rad
</td>
        <td>
1.46
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
rad
</td>
        <td>
2.19
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
sal
</td>
        <td>
0.05
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
sal
</td>
        <td>
0.09
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
sal
</td>
        <td>
0.1
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
sal
</td>
        <td>
0.21
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
        <td>
temp
</td>
        <td>
-16
</td>
    </tr>
    <tr>
        <td>
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
        <td>
rad
</td>
        <td>
11.25
</td>
    </tr>
    <tr>
        <td>
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
        <td>
sal
</td>
        <td>
22.5
</td>
    </tr>
    <tr>
        <td>
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
        <td>
sal
</td>
        <td>
41.6
</td>
    </tr>  
</table>

</div>


<div>
<p>Having all the information in one tables creates a lot of duplicate data. Now, if we want to update 'William''s name to 'Bill', we'd have to maek four (4) edits to the database.</p>
<p>Instead, lets store the survey readings in a separate table</p>
</div>


<div>
<table>
<td>
<strong>Person</strong>
<table>
    <tr>
        <th>
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td>
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td>
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td>
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td>
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td>
danforth
</td>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>
</td>

<td>

<strong>Survey</strong>
<table>
  <tr> <th>
quant
</th> <th>
reading
</th> </tr>
  <tr> <td>
rad
</td> <td>
9.82
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.13
</td> </tr>
  <tr> <td>
rad
</td> <td>
7.8
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td>
rad
</td> <td>
8.41
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.05
</td> </tr>
  <tr> <td>
temp
</td> <td>
-21.5
</td> </tr>
  <tr> <td>
rad
</td> <td>
7.22
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.06
</td> </tr>
  <tr> <td>
temp
</td> <td>
-26.0
</td> </tr>
  <tr> <td>
rad
</td> <td>
4.35
</td> </tr>
  <tr> <td>
temp
</td> <td>
-18.5
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.1
</td> </tr>
  <tr> <td>
rad
</td> <td>
2.19
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td>
temp
</td> <td>
-16.0
</td> </tr>
  <tr> <td>
sal
</td> <td>
41.6
</td> </tr>
  <tr> <td>
rad
</td> <td>
1.46
</td> </tr>
  <tr> <td>
sal
</td> <td>
0.21
</td> </tr>
  <tr> <td>
sal
</td> <td>
22.5
</td> </tr>
  <tr> <td>
rad
</td> <td>
11.25
</td> </tr>
</table>

</td>
</table>

</div>


<div>
<p>But now how will we know which reading was taken by which person? We can take the key we added to the Person table, and add the same value to a field in the Survey table to link the readings to a person.</p>
</div>


<div>
<table>
<td>
<span style="background:cyan"><strong>Person</strong></span>: people who took the readings
<table>
    <tr>
        <th bgcolor="cyan">
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td bgcolor="cyan">
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
danforth
</td>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>

</td>

<td>

<strong>Survey</strong>: the actual readings
<table>
  <tr> <th bgcolor="cyan">
person
</th> <th>
quant
</th> <th>
reading
</th> </tr>
  <tr> <td bgcolor="cyan">
dyer
</td> <td>
rad
</td> <td>
9.82
</td> </tr>
  <tr> <td bgcolor="cyan">
dyer
</td> <td>
sal
</td> <td>
0.13
</td> </tr>
  <tr> <td bgcolor="cyan">
dyer
</td> <td>
rad
</td> <td>
7.8
</td> </tr>
  <tr> <td bgcolor="cyan">
dyer
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
8.41
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.05
</td> </tr>
  <tr> <td bgcolor="cyan">
pb
</td> <td>
temp
</td> <td>
-21.5
</td> </tr>
  <tr> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
7.22
</td> </tr>
  <tr> <td bgcolor="cyan">
 
</td> <td>
sal
</td> <td>
0.06
</td> </tr>
  <tr> <td bgcolor="cyan">
 
</td> <td>
temp
</td> <td>
-26.0
</td> </tr>
  <tr> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
4.35
</td> </tr>
  <tr> <td bgcolor="cyan">
pb
</td> <td>
temp
</td> <td>
-18.5
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.1
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
rad
</td> <td>
2.19
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
temp
</td> <td>
-16.0
</td> </tr>
  <tr> <td bgcolor="cyan">
roe
</td> <td>
sal
</td> <td>
41.6
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
rad
</td> <td>
1.46
</td> </tr>
  <tr> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.21
</td> </tr>
  <tr> <td bgcolor="cyan">
roe
</td> <td>
sal
</td> <td>
22.5
</td> </tr>
  <tr> <td bgcolor="cyan">
roe
</td> <td>
rad
</td> <td>
11.25
</td> </tr>
</table>


</td>
</table>

</div>


<div>
<p>The person field in the Survey table is a special key that links each reading to a specific record in the Person table. This kind of key is called a <strong>foreign key</strong></p>
<p>Now we can add another table including information when readings were taken at specific sites. This information will be placed in a new table called Visited with a primary key called ident. In the Survey table, we will add a field (foreign key) called taken to link the site and date information to the readings.</p>
</div>


<div>
<table>
<td>
<span style="background:cyan"><strong>Person</strong></span>: people who took the readings
<table>
    <tr>
        <th bgcolor="cyan">
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td bgcolor="cyan">
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
danforth
</td>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>


<p><span style="background:yellow"><strong>Visited</strong></span>: when readings were taken at specific sites.</p>
<table>
  <tr> <th bgcolor="yellow">
ident
</th> <th>
site
</th> <th>
dated
</th> </tr>
  <tr> <td bgcolor="yellow">
619
</td> <td>
DR-1
</td> <td>
1927-02-08
</td> </tr>
  <tr> <td bgcolor="yellow">
622
</td> <td>
DR-1
</td> <td>
1927-02-10
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td>
DR-3
</td> <td>
1939-01-07
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td>
DR-3
</td> <td>
1930-01-12
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td>
DR-3
</td> <td>
1930-02-26
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td>
DR-3
</td> <td>
 
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td>
MSK-4
</td> <td>
1932-01-14
</td> </tr>
  <tr> <td bgcolor="yellow">
844
</td> <td>
DR-1
</td> <td>
1932-03-22
</td> </tr>
</table>


</td>

<td>

<strong>Survey</strong>: the actual readings
<table>
  <tr> <th bgcolor="yellow">
taken
</th> <th bgcolor="cyan">
person
</th> <th>
quant
</th> <th>
reading
</th> </tr>
  <tr> <td bgcolor="yellow">
619
</td> <td bgcolor="cyan">
dyer
</td> <td>
rad
</td> <td>
9.82
</td> </tr>
  <tr> <td bgcolor="yellow">
619
</td> <td bgcolor="cyan">
dyer
</td> <td>
sal
</td> <td>
0.13
</td> </tr>
  <tr> <td bgcolor="yellow">
622
</td> <td bgcolor="cyan">
dyer
</td> <td>
rad
</td> <td>
7.8
</td> </tr>
  <tr> <td bgcolor="yellow">
622
</td> <td bgcolor="cyan">
dyer
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
8.41
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.05
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="cyan">
pb
</td> <td>
temp
</td> <td>
-21.5
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
7.22
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="cyan">
 
</td> <td>
sal
</td> <td>
0.06
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="cyan">
 
</td> <td>
temp
</td> <td>
-26.0
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
4.35
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="cyan">
pb
</td> <td>
temp
</td> <td>
-18.5
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.1
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
lake
</td> <td>
rad
</td> <td>
2.19
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
lake
</td> <td>
temp
</td> <td>
-16.0
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
roe
</td> <td>
sal
</td> <td>
41.6
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="cyan">
lake
</td> <td>
rad
</td> <td>
1.46
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.21
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="cyan">
roe
</td> <td>
sal
</td> <td>
22.5
</td> </tr>
  <tr> <td bgcolor="yellow">
844
</td> <td bgcolor="cyan">
roe
</td> <td>
rad
</td> <td>
11.25
</td> </tr>
</table>

</td>
</table>

</div>


<div>
<p>And finally we can add a table describing each of the sites</p>
</div>


<div>
<table>
<td>
<span style="background:cyan"><strong>Person</strong></span>: people who took the readings
<table>
    <tr>
        <th bgcolor="cyan">
ident
</th>
        <th>
Personal
</th>
        <th>
Family
</th>
    </tr>
    <tr>
        <td bgcolor="cyan">
dyer
</td>
        <td>
William
</td>
        <td>
Dyer
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
pb
</td>
        <td>
Frank
</td>
        <td>
Pabodie
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
lake
</td>
        <td>
Anderson
</td>
        <td>
Lake
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
roe
</td>
        <td>
Valentina
</td>
        <td>
Roerich
</td>
    </tr>
    <tr>
        <td bgcolor="cyan">
danforth
</td>
        <td>
Frank
</td>
        <td>
Danforth
</td>
    </tr>   
</table>



<p><span style="background:pink"><strong>Site</strong></span>: locations where readings were taken.</p>
<table>
  <tr> <th bgcolor="pink">
name
</th> <th>
lat
</th> <th>
long
</th> </tr>
  <tr> <td bgcolor="pink">
DR-1
</td> <td>
-49.85
</td> <td>
-128.57
</td> </tr>
  <tr> <td bgcolor="pink">
DR-3
</td> <td>
-47.15
</td> <td>
-126.72
</td> </tr>
  <tr> <td bgcolor="pink">
MSK-4
</td> <td>
-48.87
</td> <td>
-123.4
</td> </tr>
</table>


<p><span style="background:yellow"><strong>Visited</strong></span>: when readings were taken at specific sites.</p>
<table>
  <tr> <th bgcolor="yellow">
ident
</th> <th bgcolor="pink">
site
</th> <th>
dated
</th> </tr>
  <tr> <td bgcolor="yellow">
619
</td> <td bgcolor="pink">
DR-1
</td> <td>
1927-02-08
</td> </tr>
  <tr> <td bgcolor="yellow">
622
</td> <td bgcolor="pink">
DR-1
</td> <td>
1927-02-10
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="pink">
DR-3
</td> <td>
1939-01-07
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="pink">
DR-3
</td> <td>
1930-01-12
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="pink">
DR-3
</td> <td>
1930-02-26
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="pink">
DR-3
</td> <td>
 
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="pink">
MSK-4
</td> <td>
1932-01-14
</td> </tr>
  <tr> <td bgcolor="yellow">
844
</td> <td bgcolor="pink">
DR-1
</td> <td>
1932-03-22
</td> </tr>
</table>


</td>

<td>

<strong>Survey</strong>: the actual readings
<table>
  <tr> <th bgcolor="yellow">
taken
</th> <th bgcolor="cyan">
person
</th> <th>
quant
</th> <th>
reading
</th> </tr>
  <tr> <td bgcolor="yellow">
619
</td> <td bgcolor="cyan">
dyer
</td> <td>
rad
</td> <td>
9.82
</td> </tr>
  <tr> <td bgcolor="yellow">
619
</td> <td bgcolor="cyan">
dyer
</td> <td>
sal
</td> <td>
0.13
</td> </tr>
  <tr> <td bgcolor="yellow">
622
</td> <td bgcolor="cyan">
dyer
</td> <td>
rad
</td> <td>
7.8
</td> </tr>
  <tr> <td bgcolor="yellow">
622
</td> <td bgcolor="cyan">
dyer
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
8.41
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.05
</td> </tr>
  <tr> <td bgcolor="yellow">
734
</td> <td bgcolor="cyan">
pb
</td> <td>
temp
</td> <td>
-21.5
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
7.22
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="cyan">
 
</td> <td>
sal
</td> <td>
0.06
</td> </tr>
  <tr> <td bgcolor="yellow">
735
</td> <td bgcolor="cyan">
 
</td> <td>
temp
</td> <td>
-26.0
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="cyan">
pb
</td> <td>
rad
</td> <td>
4.35
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="cyan">
pb
</td> <td>
temp
</td> <td>
-18.5
</td> </tr>
  <tr> <td bgcolor="yellow">
751
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.1
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
lake
</td> <td>
rad
</td> <td>
2.19
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
lake
</td> <td>
temp
</td> <td>
-16.0
</td> </tr>
  <tr> <td bgcolor="yellow">
752
</td> <td bgcolor="cyan">
roe
</td> <td>
sal
</td> <td>
41.6
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="cyan">
lake
</td> <td>
rad
</td> <td>
1.46
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="cyan">
lake
</td> <td>
sal
</td> <td>
0.21
</td> </tr>
  <tr> <td bgcolor="yellow">
837
</td> <td bgcolor="cyan">
roe
</td> <td>
sal
</td> <td>
22.5
</td> </tr>
  <tr> <td bgcolor="yellow">
844
</td> <td bgcolor="cyan">
roe
</td> <td>
rad
</td> <td>
11.25
</td> </tr>
</table>

</td>
</table>

</div>


<div>
<p>Here is our final database that we will be running queries against for the rest of the workshop</p>
</div>


<div class="in">
<pre>!sqlite3 survey.db &lt; gen-survey-database.sql</pre>
</div>


<div>
<table>
<tr>
<td valign="top">
<p><strong>Person</strong>: people who took readings.</p>
<table>
  <tr> <th>
ident
</th> <th>
personal
</th> <th>
family
</th> </tr>
  <tr> <td>
dyer
</td> <td>
William
</td> <td>
Dyer
</td> </tr>
  <tr> <td>
pb
</td> <td>
Frank
</td> <td>
Pabodie
</td> </tr>
  <tr> <td>
lake
</td> <td>
Anderson
</td> <td>
Lake
</td> </tr>
  <tr> <td>
roe
</td> <td>
Valentina
</td> <td>
Roerich
</td> </tr>
  <tr> <td>
danforth
</td> <td>
Frank
</td> <td>
Danforth
</td> </tr>
</table>

<p><strong>Site</strong>: locations where readings were taken.</p>
<table>
  <tr> <th>
name
</th> <th>
lat
</th> <th>
long
</th> </tr>
  <tr> <td>
DR-1
</td> <td>
-49.85
</td> <td>
-128.57
</td> </tr>
  <tr> <td>
DR-3
</td> <td>
-47.15
</td> <td>
-126.72
</td> </tr>
  <tr> <td>
MSK-4
</td> <td>
-48.87
</td> <td>
-123.4
</td> </tr>
</table>

<p><strong>Visited</strong>: when readings were taken at specific sites.</p>
<table>
  <tr> <th>
ident
</th> <th>
site
</th> <th>
dated
</th> </tr>
  <tr> <td>
619
</td> <td>
DR-1
</td> <td>
1927-02-08
</td> </tr>
  <tr> <td>
622
</td> <td>
DR-1
</td> <td>
1927-02-10
</td> </tr>
  <tr> <td>
734
</td> <td>
DR-3
</td> <td>
1939-01-07
</td> </tr>
  <tr> <td>
735
</td> <td>
DR-3
</td> <td>
1930-01-12
</td> </tr>
  <tr> <td>
751
</td> <td>
DR-3
</td> <td>
1930-02-26
</td> </tr>
  <tr> <td>
752
</td> <td>
DR-3
</td> <td bgcolor="red">
 
</td> </tr>
  <tr> <td>
837
</td> <td>
MSK-4
</td> <td>
1932-01-14
</td> </tr>
  <tr> <td>
844
</td> <td>
DR-1
</td> <td>
1932-03-22
</td> </tr>
</table>
</td>
<td valign="top">
<p><strong>Survey</strong>: the actual readings.</p>
<table>
  <tr> <th>
taken
</th> <th>
person
</th> <th>
quant
</th> <th>
reading
</th> </tr>
  <tr> <td>
619
</td> <td>
dyer
</td> <td>
rad
</td> <td>
9.82
</td> </tr>
  <tr> <td>
619
</td> <td>
dyer
</td> <td>
sal
</td> <td>
0.13
</td> </tr>
  <tr> <td>
622
</td> <td>
dyer
</td> <td>
rad
</td> <td>
7.8
</td> </tr>
  <tr> <td>
622
</td> <td>
dyer
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td>
734
</td> <td>
pb
</td> <td>
rad
</td> <td>
8.41
</td> </tr>
  <tr> <td>
734
</td> <td>
lake
</td> <td>
sal
</td> <td>
0.05
</td> </tr>
  <tr> <td>
734
</td> <td>
pb
</td> <td>
temp
</td> <td>
-21.5
</td> </tr>
  <tr> <td>
735
</td> <td>
pb
</td> <td>
rad
</td> <td>
7.22
</td> </tr>
  <tr> <td>
735
</td> <td bgcolor="red">
 
</td> <td>
sal
</td> <td>
0.06
</td> </tr>
  <tr> <td>
735
</td> <td bgcolor="red">
 
</td> <td>
temp
</td> <td>
-26.0
</td> </tr>
  <tr> <td>
751
</td> <td>
pb
</td> <td>
rad
</td> <td>
4.35
</td> </tr>
  <tr> <td>
751
</td> <td>
pb
</td> <td>
temp
</td> <td>
-18.5
</td> </tr>
  <tr> <td>
751
</td> <td>
lake
</td> <td>
sal
</td> <td>
0.1
</td> </tr>
  <tr> <td>
752
</td> <td>
lake
</td> <td>
rad
</td> <td>
2.19
</td> </tr>
  <tr> <td>
752
</td> <td>
lake
</td> <td>
sal
</td> <td>
0.09
</td> </tr>
  <tr> <td>
752
</td> <td>
lake
</td> <td>
temp
</td> <td>
-16.0
</td> </tr>
  <tr> <td>
752
</td> <td>
roe
</td> <td>
sal
</td> <td>
41.6
</td> </tr>
  <tr> <td>
837
</td> <td>
lake
</td> <td>
rad
</td> <td>
1.46
</td> </tr>
  <tr> <td>
837
</td> <td>
lake
</td> <td>
sal
</td> <td>
0.21
</td> </tr>
  <tr> <td>
837
</td> <td>
roe
</td> <td>
sal
</td> <td>
22.5
</td> </tr>
  <tr> <td>
844
</td> <td>
roe
</td> <td>
rad
</td> <td>
11.25
</td> </tr>
</table>
</td>
</tr>
</table>

</div>


<div>
<p>Notice that three entries—one in the <code>Visited</code> table, and two in the <code>Survey</code> table—are shown in red because they don't contain any actual data: we'll return to these missing values <a href="#s:null">later</a>.</p>
</div>


<div>
<h4 id="challenges">Challenges</h4>
<ol style="list-style-type: decimal">
<li>If we had data for the time each of the visits occured, where would you add it?</li>
</ol>
</div>


<div class="keypoints">
<h4 id="key-points">Key Points</h4>
<ul>
<li>A relational database stores information in tables, each of which has a fixed set of columns and a variable number of records.</li>
<li>A database manager is a program that manipulates information stored in a database.</li>
<li>We write queries in a specialized language called SQL to extract information from databases.</li>
<li>SQL is case-insensitive.</li>
</ul>
</div>
