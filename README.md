# Book Management System
 
 >> Server
    >>Storing Book Data
    >> User Registration 
    >>Subscription
# Routes and Endpoints

## /users
GET: Get all list of the users
Post: Create a new user

## /users/{id}
Get:Get all the user information for specific user by their id
Put: Update the user information
Delete: Delete the user(check if they stil have an issued book and is there any fine to be collected from them)

Subscription:

    >> 3 months(basic subscription)
    >> 6 months(Standard Subscription)
    >> 1 year(Premium Subscription)

## /users/subscription-details/{id}
Get:Get user subscription details
    >> Date of Subscription
    >> Valid till
    >> Fine if any

## /books
Get: Get all the books
Post: Add a new book

## /books/{id}
Get:Get the book information for specific book by their id
Put: Update the book information by ID

## /books/issued
Get: get all issued books

## /books/issuedbooks/withfine
Get:Get all issued books for specific user by their id

# Fine Calculation
>> If the user has issued a books and the issued book is to returned at 01/01/2024 if he missed the date of renewal or subscription date expires  then he needs to pay the penalty of rs. 200/-
