# ChapChap SQL Operations
A light weight PHP library for performing brisk SQL operations.
-------------------------------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------------------------------
### ☲ ChapChapSQL v2.0.0                                                                                              
-------------------------------------------------------------------------------------------------------------------
* Created by [Kelvin Kamau](https://www.kelvinkamau.com) & Flavia Mbuki                                                     
* Distributed under the Open Source License                                                            
-------------------------------------------------------------------------------------------------------------------

## 0. FOREWORD:
  - This library is created with the objective of reducing the amount of code one has to write in order to connect to and perform operations on a database.
      e.g. to select data from a database in a specific format or update the data in a database table.
  - To achieve this, the library uses the PDO approach and an object-oriented approach in the PHP Language.
  - Security is a major concern, and thus major steps are taken to achieve this;
      e.g. use of Prepared Statements, and escaping data before each database operation is executed.
  - Note that in functions which return data from the database, the data is returned in a 2D array. Do a loop to get individual data (examples are given).
      e.g. in ```sql 'select()' && 'select2()' functions. ```

## 1. USE:
 ### 1.1 Getting Started - Setting up a sample environment
  - To use this library, you need a sample database. An example has been provided in the root directory (sample_db.sql)
  - Simply create a new database in your server, and import the file 'sample_db.sql'. Note that for my environment, am using PHP Version: 7.0.8
  - The 'core' folder contains a database connection file, and a file with functions for executing swift database functions.
  - Update the credentials in the 'db_connect.php' to match the ones in your local server so as to allow a successful database connection.
  - The 'core' folder contains two versions of the main library, 'chapchap_sql.php' - use the minimized version for production and the latter for development purposes.

  ### 1.2 Using & Reusing The code
  - In the root folder, the file 'index.php' contains sample code that illustrate the using of this library.
  - To illustrate a function's usage, simply uncomment the lines of code which follow the line commented out as /* .. */ 
  e.g 
  
  ```sql
  1. /* SELECT column_names FROM table_name */
  2. // $query = select("hello_world", ['id', 'name', 'random'], []);
  3. // print_results($query);
  ```
  
  Here, simply uncomment the second & third lines (the lines commented out with a '//')
  - To reuse the code, all you need is a copy of the main library 'chapchap_sql.php' and the connection file.

## 2. HELP & CONTRIBUTIONS:
  - If you have any questions regarding this library or how to use it, simply get in touch with me via Email holla@kelvinkamau.com.
  - This is an open source project; as such, contributions are highly appreciated and welcome.
  - If you need to make a contribution to this project, simply make a pull request on the Github folder.
  - The main library will be updated to reflect all helpful contributions, and the contributors will be duly recognized.
  
 ## 3. SPECIAL THANKS
  - Thanks to my partner Flavia Macharia ❤ for her unbowing support, great insight and contribution.
  
  ## 4. LICENSE
  ``` MIT License

Copyright (c) 2017 Kelvin Kamau & Flavia Macharia

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE. 
  
