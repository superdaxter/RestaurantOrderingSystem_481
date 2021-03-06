# Resturant Ordering System  

Created by: Mehrad Faridan, Ronan Rank-Nemish, Ace Saspa, and Jesse Zheng.

## Running program

To run the code:

1. Open 'RestaurantOrderingSystem_481.sln' in the 'RestaurantOrderingSystem_481' folder.

2. Click the Green play button at the top to run the program.

## Functionality implemented (that affect more than just one page).

Functions not mentioned here are mentioned under the "Using the system" heading.

    - All buttons (except the language buttons) will make some visual change (opening/closing pop-up, changing the page, changing the window).

    - Popups are simulated by having other windows appear.

    - All quantities do not go below 1.

    - Then the quantity of items is 1 the '-' button will not be shown. When the quantity is greater than 1 it appears.

    - Entering or changing the table number will change the number for anywhere it appears.

    - Adding/removing/changing quantity of items in the cart will update everywhere it's needed (Cart page and Checkout page).

    - The Cowboy burger selection screen (as seen in the video at 2:44) was only hard-coded and not implemented with the system. Inside the Visual Studio it is saved as "ItemSubstitution.xaml" and "ItemSubstitution.xaml.cs" 

## Using the system

For each page, the instructions for what everything on the page does is explained; then any functions not explained in the instructions or the above heading (Functionality implemented) are explained.

1. Landing page

    Instructions:

        - Enter a number between 1 and 100 under where is says 'Enter Your Table Number:'

        - Press 'OK' to proceed to Menu page.

        - You can change the language using the two buttons on the bottom left (No vertical implementation).

2. Menu page

    Instructions:

        - There is a button at the top left of the window that contains the table number. This button can be tapped to change the current table number. A pop-up will appear prompting the user to enter a table number the pop-up does the following:
            
            - The 'X' button will close the pop-up (and nothing will change). 
            
            - If a number between 1-100 is entered, then the 'Change' button is pressed, the table number will change. Otherwise, the pop-up will close and nothing will change.

        - Search through the menu by scrolling and selecting from the five categories on the left (the buttons 'Appesisers' to 'Slides'). 

        - When you tap a menu item, a pop-up will appear. It does the following: 

            - The 'X' button at the top right will close the pop-up and nothing will happen.
            
            - In the pop-up, you can type in a special request with this item. 
            
            - You can change the quantity with the '+' and '-' buttons. The '-' button will appear if the quantity is greater than 1. 
            
            - The 'Add to Cart' button will then add the item to the cart. The pop-up will then close.

        - Pressing the red 'Call Server' button allows calling a server over to talk to them (No vertical implementation). A popup will appear indicating a server has been called; it will disappear shortly after.

        - You can tap the cart icon at the bottom of the screen to pull up the Cart page. 

        - The checkout button is at the bottom right of the screen to checkout the items in the cart. It will lead to the Checkout page

        - If an order is already made, a 'Previous Order' button will appear at the top right of the screen to go back to the Finalize page.

    Other functionality:

        - The 'Previous Order' button does not appear on the Menu page until after an order has been made.

        - Tapping through the food categories (Appetisers, Entrees, etc.) will change what items appear on the menu.

        - There is a scroll bar at the right of the screen if the items in the menu go off the screen.

        - Tapping anywhere inside the rectange for each item will bring up the pop-up to add it to cart.

        - Pressing the cart icon button simulates the cart pulling out from the bottom of the screen.

        - The current total cost (without tax) appears at the bottom left of the screen and changes dynamically based on what items (and their quantity) are in the cart.

3. Cart page

    Instructions:

        - The ability change to the table number and to go back to the Finalize page (if an order is already made) is available at the top of the screen, same functionality as mentioned for the Menu page.

        - The button with the arrow will close the cart and return to the Menu page.

        - If any items are in the cart they will appear under the arrow. Items in the cart have the following fuctionality:

            - The trash icon on the left of each item in the cart can be used to remove items.

            - The '+' and '-' button can be used to increase or decrease the respective item's quantity. The '-' button will not appear when the quantity is 1.

            - If any special requests were made, they will appear under the name of the item.

        - There is a 'Checkout' button at the bottom right that leads to the Checkout page.

    Other functionality:

        - Pressing the arrow simulates the Cart page sliding down.

4. Checkout page

    Instructions:

        - A 'Back' button will be at the top left of the screen that leads back to the Menu page.

        - The ETA for food is at top right of screen (hard-coded to 30 min).

        - Any items in the cart will appear below "Menu Items:". They do the following:

            - Buttons for items in the cart work the same as mentioned on the Cart page (trash icon removes item, '+' and '-' change quantity, special requests appear under the name of item).
        
        - The 'Confirm Order' button opens a pop-up. The pop-up does the following:

            - The 'X' closes the pop-up and nothing else happens.

            - Pressing 'Confirm Order' takes you to the finalize page.

5. Finalize page

    Instructions:

        - The ETA is still at the top right of the screen.

        - The 'Call Server' button has the same functionality as mentioned for Menu page.

        - The 'Order More' button brings the user back to the Menu page to order more food. A 'Previous Order' button will appear at the top right of the Menu when this is done to return to the Finalize page.

        - The 'Request Takeout Boxes' button brings up a pop-up that does the following:

            - Anything done in this pop-up doesn't affect the system in any way.
            
            - The 'X' button closes the pop-up.

            - A quantity will appear in the middle of the screen with a '+' and '-' button on either side. These buttons can be used to change the quantity.

            - The 'Submit' button closes the pop-up.

        - The 'Review Order' button opens a pop-up that contains your last order submitted. On it there is an 'X' button to close the pop-up.

        - The 'Leave Us A Review!' button brings up a pop-up with the following:

            - Anything done on this pop-up doesn't affect the system.

            - The 'X' button at the top right closes the pop-up.

            - Only one of the radio buttons can be selected.

            - The text box below the radio buttons is for any comments about the review.

            - The 'Submit' button closes the pop-up.

## Walkthrough

This walkthrough will go through the basic process to order a few items. It assumes the system is currently running. To see how to do this, refer to the "Running program" heading.

1. Enter a number between 1 and 100 below where it says 'Enter Your Table Number:'.

2. Press 'OK'. 
    
    - This will bring you to the Menu page. To see a list of all the features and functions on this page, take a look at the "Using the system" heading above.

3. Press the pink box with the heading 'Caesar Salad'.

    - This brings up a pop-up.

4. Press the '+' button once to increase the quantity to 2.

5. Press the 'Add to Cart' button to add the dish to cart.

6. Select the 'Entrees' tab on the left of the screen to look at entrees.

7. Press the pink box with the heading 'Canadian Prime Sirloin'.

    - This brings up a pop-up.

8. Type in the text box "Extra Mashed Potatos" to request extra mashed potatos.

9. Press 'Add to Cart' to add the dish to cart.

10. Press the button with the cart icon at the bottom of the screen to view cart.

    - This will bring you to the Cart page. To see a list of all the features and functions on this page, take a look at the "Using the system" heading above.

11. Press the 'Checkout' button at the bottom right of the screen to verify your cart.

    - This will bring you to the CHeckout page. To see a list of all the features and functions on this page, take a look at the "Using the system" heading above.

12. Press the '+' button next to 'Canadian Prime Sirloin' to increase the quanitity once.

13. Press 'Confirm Order' to send it to the kitchen.

    - A pop-up will appear to notify the customer to order at the same time if they are with other people for the best restaurant experience.

14. Press 'Confirm Order' on the pop-up. The order is then sent to the kitchen.

15. Press 'Order More' to order more food. Repeat steps 3-14.

    - *Now you've finished eating.*

16. Press 'Request Takeout Boxes' to request takeout boxes.

    - This brings up a pop-up.

17. Press '+' once to increase quantity to 2.

18. Press 'Submit' to send the request to the staff.

    - A pop-up will appear to notify the request was sent. It will close shortly.

19. Press 'Leave Us A Review!' to leave a review.

    - A pop-up will appear.

20. Press the radio button under '5'.

21. Type in "Excellent!" in the text box.

22. Press 'Submit' to send the review.

23. Press 'Call Server' to request the bill.

    - A pop-up will appear notifying the request has been sent. It will close shortly.

24. You are done! :D


## Video summary

The benefits of the system are mentioned, followed by 2 user stories that walk through the system. The timestamps for noteworthy events and features are included below.

- 0:00 Introduction

- 0:22 Benefits of the system

- 0:54 User story (Jessica, single vegetarian mom)

- 1:04 Table number entered

- 1:17 Filter icons explained

- 1:29 Special request made

- 1:33 Browsing cart

- 1:40 Quantity increased from within cart

- 1:45 ETA explained

- 1:57 Server called to get bill

- 2:10 End of user story (Jessica)

- 2:15 User story (Barry, banker, fine diner)

- 2:21 Languages mentioned

- 2:30 Wrong table number entered

- 2:37 Wrong characters entered

- 2:44 Cowboy burger selection

- 2:47 Server called to ask question

- 3:14 Takeout box requested

- 3:17 More food ordered

- 3:20 Alcohol ordered

- 3:25 Alcohol age verification

- 3:40 Left review

- 4:03 End of user story (Barry)