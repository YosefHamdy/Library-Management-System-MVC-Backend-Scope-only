# LibraryMS
Library management system in "MVC" architectural pattern using "Hibernate" ,"Java" ,"OracleDB"

## Classes

User :' Which is the Superclass that have common intialization of fields that will be used in other users'

Customer  : 'Inherit the User Attributes '
Customer Services : 'Contain implementation of customer method'

Librarian : 'Inherit the User Attributes '
Librarian Services : 'Contain implementation of Librarian method'

Publisher :'Inherit the User Attributes '
Publisher Services : 'Contain implementation of Publisher method'

Books : 'Contain book fields definition and Mapping between other classes'
BookServices 


App : 'Which is the main and Contains Calling and use services methods '

### Relations Between classes

One to Many : 'Librarian to Customer'
              'Librarian To Books'
              'Librarian To Publisher'
              'Customer To Books'
            
Many to one : 'Books to Customer<To prevent made a separate table>'
  
Many to Many : 'Publisher to Books' 


#### Related DB Tables for Each Class
  
Librarian : -- Librarian,Added_Books , Added_Clients
 
Customer  : -- Customer,Books 

Publisher : -- Publisher,Publisher_Books 
  
