# Bootstrap-tables-cards


This is intended as a quick reference and showcase for Bootstrap4 Tables and Cards


## Table of Contents

 - Bootstrap Tables
 - Responsive Tables
 - Table hover
 - Boredered Table
 - Bootstrap Cards
 - Cards views
 - Card header
 - Card body
 - Card footer


### Table

As we know bootstrap is a framework.it consists number of default classes to get intereact response in the webpage.In this scenario to get table format in webpage we have to use .table class as parent class based upon our requirement we will use sub classes.


```html
<table class="table">
  <thead>
    <tr>
      <th scope="col">S.No</th>
      <th scope="col">First_Name</th>
      <th scope="col">Last_Name</th>
      <th scope="col">Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Warren </td>
      <td>Buffett</td>
      <td>89</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jeff </td>
      <td>Bezos</td>
      <td>56</td>
    </tr>
   
  </tbody>
</table>
```
Output:

![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/img1.PNG "Output 1")


- If we see table structure it can be divided in to 3 tags :

  -  ```<thead></thead>``` - heading content can be include in this tag
  -  ```<tbody> </tbody>``` - main content respective heading can be includ in this tag
  -  ```<tfoot> </tfoot>``` - content which can be shown in bottom of the table can include in this tag

- Sub tags of table tag :
  - ```<tr></tr>``` for display data in row
  - ```<th></th>```  Defines a header cell whether it is a row|column|group of rows|group of columns
  - ```<td></td>```  for display data in cell of a table
  
Lets see some attributes for th tag: scope, colspan and rowspan

```<th scope="col|row|colgroup|rowgroup" colspan="2" rowspan="3">```

Scope:The scope attribute has no visual effect in ordinary web browsers,
 but can be used by screen readers.

- Attribute values for scope:
  - col-Specifies that the cell is a header for a column
  - row-Specifies that the cell is a header for a row
  - colgroup-Specifies that the cell is a header for a group of columns
  - rowgroup-Specifies that the cell is a header for a group of rows
  - colspan - cell spans multiple number of columns 
  - rowspan - cell spans multiple number of rows 
  ```
  <table class="table" border="1">
        <thead>
          <tr>
            <th scope="col">Poster name</th>
            <th scope="col">Color</th>
            <th colspan="3">Sizes available</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th rowspan="3">Zodiac</th>
            <th scope="row">Full color</th>
            <td>Medium</td>
            <td>Large</td>
            <td>X-large</td>
          </tr>
          <tr>
            <th scope="row">Full color</th>
            <td>Medium</td>
            <td>Large</td>
            <td>X-large</td>
          </tr><tr>
          <th scope="row">Full color</th>
          <td>Medium</td>
          <td>Large</td>
          <td>X-large</td>
        </tr>
      </tbody>
    </table> 
    ```
    Output:

![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/img2.PNG "Output for <th> attributes")


Contextual Classes:
-------------------
Contextual classes can be used to color the table,table rows or table cells. 
The classes that can be used are: 
- .table-primary,
- .table-success,
- .table-info,
- .table-warning,
- .table-danger, 
- .table-active,
- .table-secondary, 
- .table-light and .table-dark

 Output:
![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/table.PNG "Output for contextual classes")



Striped rows
Use .table-striped to add zebra-striping to any table row within the <tbody>.
 ```
 <table class="table table-striped">
  <thead>
    <tr>
      <th scope="col">S.No</th>
      <th scope="col">First_Name</th>
      <th scope="col">Last_Name</th>
      <th scope="col">Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Warren </td>
      <td>Buffett</td>
      <td>89</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jeff </td>
      <td>Bezos</td>
      <td>56</td>
    </tr>
   <tr>
       <th scope="row">3</th>
       <td>Mark </td>
       <td>Zuckerberg</td>
       <td>35</td>
    </tr>
   </tbody>
</table>
```

   Output:

![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/strip.PNG "Output for striped rows")


Bordered table
Add .table-bordered for borders on all sides of the table and cells.

```

<table class="table table-bordered">
  <thead>
    <tr>
      <th scope="col">S.No</th>
      <th scope="col">First_Name</th>
      <th scope="col">Last_Name</th>
      <th scope="col">Age</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">1</th>
      <td>Warren </td>
      <td>Buffett</td>
      <td>89</td>
    </tr>
    <tr>
      <th scope="row">2</th>
      <td>Jeff </td>
      <td>Bezos</td>
      <td>56</td>
    </tr>
   <tr>
      <th scope="row">3</th>
      <td>Mark </td>
      <td>Zuckerberg</td>
      <td>35</td>
   </tr>
 </tbody>
</table>
```
 Output:
![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/img4.PNG "Output for bordered class")


Hoverable rows
Add .table-hover to enable a hover state on table rows within a <tbody>.
```
  <table class="table table-hover">
        <thead>
          <tr>
            <th scope="col">S.No</th>
            <th scope="col">First_Name</th>
            <th scope="col">Last_Name</th>
            <th scope="col">Age</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <th scope="row">1</th>
            <td>Warren </td>
            <td>Buffett</td>
            <td>89</td>
          </tr>
          <tr>
            <th scope="row">2</th>
            <td>Jeff </td>
            <td>Bezos</td>
            <td>56</td>
          </tr>
        </tbody>
        <tfoot>
         <tr>
          <th scope="row">3</th>
          <td>Mark </td>
          <td>Zuckerberg</td>
          <td>35</td>
        </tr>
         </tfoot> 
    </table> 
    ```
 output:
 ![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/hover.PNG "hover")



Responsive tables:
------------------
Responsive tables allow tables to be scrolled horizontally with ease.
Make any table responsive across all viewports by wrapping a .table with .table-responsive.
Or, pick a maximum breakpoint with which to have a responsive table up to by using .table-responsive{-sm|-md|-lg|-xl}.

To get resposive for a webpage we have to include meta tag in ```<head></head>``` as shown below:

 
Code for responsive table:   
-------------------------
 ```
 <div class="table-responsive">
    <table class="table table-bordered">
      <thead>
        <tr>
          <th>#</th>
          <th>Firstname</th>
          <th>Lastname</th>
          <th>Age</th>
          <th>City</th>
          <th>Country</th>
          <th>Sex</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1</td>
          <td>Sam</td>
          <td>Beauty</td>
          <td>32</td>
          <td>Hyderabad</td>
          <td>India</td>
          <td>Female</td>
        </tr>
      </tbody>
    </table>
  </div>
```

 output:
 ![alt text](https://github.com/KalyanPaladugu/Bootstrap-tables-cards/blob/master/images/responsive.PNG "responsive")
 
 
Breakpoint specific
Use .table-responsive{-sm|-md|-lg|-xl} as needed to create responsive tables up to a particular breakpoint.
From that breakpoint and up, the table will behave normally and not scroll horizontally.

These tables may appear broken until their responsive styles apply at specific viewport widths.
