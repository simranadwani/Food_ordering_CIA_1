# Lavasa Food Ordering System

## Programmed by
1. Simran Adwani (Reg no. 22112335) (https://github.com/simranadwani)
2. Homita Ganguly (Reg no. 22112314) (https://github.com/HomitaGanguly)

## Description
This is a basic Python "food ordering project" that allows users to create a personal account and place food orders from various restaurants located in Lavasa, Pune and their menus and calculates the total cost of the order, gives the user options of view cart to view order summary, checkout to make payment and lastly an option to quit the program. The project provides a simple command-line interface (CLI) for users to interact with.

## Features
* **Allows user to login if an account exists by entering valid username and password otherwise allows user to create a personal account**
   * with unique username
   * with validated password
* **Allows user to place an order**
   * allows user to select restaurants from given options
   * allows user to select items and quantities from the available category of food and  based on the selected restaurant
   * allows user to see the order summary including specific items and their quantities and final price
   * allows uset to make payment
* **Allows user to quit the program with or without ordering any item**

## Functionality
1. **class User** : A class providing user information which includes name, adress and payment information
2. **class Order** : A class to represent the order of an user which includes user details, items and total cost
3. Packages imported: 
   * **csv**: To read and edit the "user" csv file and to read from the "menu" csv file
   * **pandas**: To display the order summary in a structured format
   * **random**: To randomly assign delivery boys and generate delivery timings.
   * **os (readlink)**: To read the value of symbolic link and return the path it points to.
   * **simple_colors**: To enhance/beautify the command line interface.
   * **tabulate**: To return the bill/order summary in a proper tabulated format.
4. Functions defined: 
   * ***Used for creating user account interface***:
      * **is_user_exists(username)**: Function defined to check whether the input username aklready exists or not. 
      * **create_user_account(x,y)** : Function defined to create a new user account incase the username/password does not exist.
      * **validate_password(password)**: Function to help users create an appropriate password by following the given rubrics.
      * **login_user(username, password)**: Function defined to finaaly let the users login through given details.
      * **account_login_or_create()**: Main function defined to print the ciommand line interface for creating an account by calling the above mentioned functions. 
   * ***Used for creating the main menu and ordering interface***:
      * **load_menu()**: Function to load the menu from the CSV file defined using for loop if conditional statements and list functions.
      * **display_categories(menu)**: Function to display the categories of food a restaurant serves defined using for loop and string function. 
      * **display_menu_items(menu, restaurant, category)**: Function to display the menu items within a category defined using for loop, string and dictionary function.  
      * **calculate_order_price(order, menu)**: Function to calculate the final order price defined using for loop, string, dictionary and list function. 
      * **view_cart(order)**: Function to view what you ordered and due payment defined using for loop, if-else conditional statements and string functions.
      * **assign_delivery_boy(delivery_boys, order)**: Function to assign random delivery boys if ordered. 
      * **checkout(order)**: Function to give payment options to users.
      * **generate_order_summary(order, delivery_boy)**: Function to generate order summary in the form of a data frame dpne using pandas package
      * **exit_program()**: Function tp exit the program (system).
      * **main()**: Main function to get the user command line interface for ordering using various options.
        
## Requirements 
1. Ensure the menu dataset file (menu.csv) is in the desired directory.
    * Columns in the csv file:
        * Restaurant
        * Category
        * Items
        * Price
3. Ensure the users dataset file (users.csv) is in the desired directory.
    * Columns in the csv file:
        * Name
        * Adress
        * Payment
        * Password
5. After importing the files make sure to run all the given codes so as to ensure installation of necessary packages.
6. Make sure to follow the prompts to ensure smooth functioning of the system.

## Usage
1. Clone this repository to your local machine or download the source code.
2. Open a terminal or command prompt and navigate to the project directory.
3. Run the command to start the food ordering system: for eg: python/conda python_mini_project.py 
4. Follow the prompts in the CLI to select the restaurant, food items, quantities to get further options.
5. Once you have completed your order, the system will keep on giving you the following options : 
   1. Browse the menu
   2. View my cart
   3. Checkout
   4. Quit
hence you can select from the options and go on to view order summary using 'view my cart' or pay using 'checkout' and lastly exit the program using 'quit' which will show you "____________________*Thank you for using our food ordering system! Please visit again!*____________________"  

## Sample Output
Here is an example of how the CLI would look:
* ***User Account***:
  
* ![image](https://github.com/HomitaGanguly/Python-CIA-1/assets/118895179/be5837c9-c305-45c1-bd44-358db9c3df8b)

* ***Order*** :
  
* ![image](https://github.com/HomitaGanguly/Python-CIA-1/assets/118895179/c8a888d4-c5d9-46d7-84df-8de1f46c2dbe)
* ![image](https://github.com/HomitaGanguly/Python-CIA-1/assets/118895179/2d10548c-9116-4a04-bfbd-272aa6a8547a)
* ![image](https://github.com/HomitaGanguly/Python-CIA-1/assets/118895179/4537dd37-f46b-4618-8b0f-0e021c1bdbf1)
* ![image](https://github.com/HomitaGanguly/Python-CIA-1/assets/118895179/9a9fc276-b45a-43e2-b8c5-830e8c2b342e)


# Thank you for viewing our project!
