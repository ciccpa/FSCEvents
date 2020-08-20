# FSCEvents
Event registration system created for Farmingdale State College (SUNY).
You can view the live site [here](fscevents.com).

This web application uses the following technologies:
- [PHP/PHP Data Objects (PDO)](https://www.php.net/manual/en/book.pdo.php).
- JavaScript
- jQuery
- AJAX

In order to run this project locally you will need the following database tables. You can download a backup of the database 
using the file: ```fsc_events_data.sql```

## Login page.
![81853347-4eb6f680-952a-11ea-8e92-132f1479b86f](https://user-images.githubusercontent.com/50625576/89063907-fc21f500-d336-11ea-99f2-f71c7b8ccdd3.png)

## Register page. 
Must have a valid FSC login to be able to register. User can register as student or faculty. 
![81853953-2d0a3f00-952b-11ea-8c25-bbb1575eee34](https://user-images.githubusercontent.com/50625576/89063714-b1a07880-d336-11ea-9e65-f8a5089b081e.png)

## Create events page. 
Must enter title, description, event type (General, Athletics, Admissions, Club, Academics, Tutoring).
If capacity is specified, event will be made available for students to register until signup limit is reached.
![81853647-b1a88d80-952a-11ea-83e1-5dcbcb9d9bc1](https://user-images.githubusercontent.com/50625576/89063846-e7ddf800-d336-11ea-8929-3f0deab183c3.png)

## My Account page. 
Lefthand side allows user to edit/enter details, righthand side displays events you've signed up for (or events you've created, if you are an admin).
![81853518-84f47600-952a-11ea-83c6-0c1f541b22fd](https://user-images.githubusercontent.com/50625576/89063871-f0cec980-d336-11ea-91a5-8b50c309ccb4.png)

## Events dashboard. 
This is where events are shown. To create an event, you must be an admin. The only way to become an admin is request administrative rights and an existing admin will have to promote your account.
![81852788-9426f400-9529-11ea-994e-5a8a8df79a09](https://user-images.githubusercontent.com/50625576/89063941-0d6b0180-d337-11ea-8aa6-5250808c851b.png)

## Known issues.

- This site has NOT yet been fully optimized for mobile devices.

- Throughout use, you may get an error that looks something like this:
``` [Warning]: PDO::__construct(): MySQL server has gone away ```
This is can be due to a number of reasons listed [here](https://dev.mysql.com/doc/refman/8.0/en/gone-away.html).
A possible solution would be to set wait_timeout when MySQL server begins. 
This is issue can be ignored and will not affect use of the project.
