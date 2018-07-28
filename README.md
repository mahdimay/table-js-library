# Table JS Library
A very simple and clean JS library to add pagination and search functionality to your table!
## Installation
To install Table JS Library, simply include the file in your project. 
## How to use
To use this library, you need to pay attention to some important notes. 
#### Table Structure
All of the TR elements in your table except the TR in THEAD needs to have a class called data.
Example:
```
<table>
<thead>
<tr>
  <th>ID</th>
  <th>Name</th>
  <th>Job</th> 
</tr>
</thead>
<tbody>
<tr class="data">
<td>1</td>
<td>John</td>
<td>Programmer</td>
</tr>
<tr class="data">
<td>2</td>
<td>Walter</td>
<td>Programmer</td>
</tr>
</table>
```
#### Pagination
This library requires you to have at least 5 buttons for pagination. This all 5 numbers need to have numbers. Starting from 1 and ending at 5. The button with number 1 needs to have id l1. The button with number 2 needs to have id l2. And this goes for button 3,4, and 5. And each li element needs to have tlist class. Example:
```
<li id="l1" class="tlist">1</li>
<li id="l2" class="tlist">2</li>
<li id="l3" class="tlist">3</li>
<li id="l4" class="tlist">4</li>
<li id="l5" class="tlist">5</li>
```
You can also add Next and Previous button to your pagination. The previous button needs to have prev id. The next button needs to have nxt id.
```
<li id="prev">Previous</li>
<li id="nxt">Next</li>
```
You can add first page and last page links. This enables your table to be more flexable. The first page id needs to be first and the last page id needs to be last.
```
<a href="#" id="first">First page</a>
<a href="#" id="last">Last page</a>
```
#### Page number
If you want your table to show what page the user is currently and how many pages are in total you need to include a div with id pagenum. Example:
```
<div id="pagenum"></div>
```
#### Search input
To enable search functionality you should add an input with id of search. Example:
```
<input id="search">
```
#### Search alert box
If no data shows up after search the library tells user why. If you want to add this alert box you need to have a div with id of alertbox. Example:
```
<div id="alertbox"></div>
```
### AND YOU ARE DONE! If you need to see the example please check sample.html file in this repository.
