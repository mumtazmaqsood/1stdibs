# stdibs
selenium + python testing www.stdibs.com

Implemented POM , CREATED SIX PAGES AND 23 TEST CASES AND GENERATED REPORTS, 
#UNITEST FRAME WORK USED 



    #--------------------------------------------------------------
    # this test click on Log In link and accept popups after log in
    #------------def test_a_login(self):---------------------------    
    Scenario:   Login to 'myAccount' 
    Given   :   On site home page
    When    :   Click on 'Log In'link on Home page
    And     :   Enter user name 'virgo4m@gmail.com'
    And     :   Enter Password  'vici2FHh'
    And     :   Click on 'Log In' Button
    Then    :   Login successfull and page redirect to home page
    #------------END test_a_login(self):---------------------------- 

#--------------------------------------------------------------------------

    #--------------------------------------------------------------------
    # this test covers TOP RIGHT MENUs
    # My Account,  Notification, My Fav, Cart 
    #------------def test_b_topRightMenu(self):---------------------------    
    Scenario:   Hower over on Top right menu on 'My Account','Notification','My Fav', 'Cart' etc 
    Given   :   On site user home page, after logging in
    When    :   on user home page, 
    And     :   Hover over 'Account Information' 
    And     :   Hover over 'Notifications'
    And     :   Hover over 'My Favorites'
    And     :   Hover over 'My Cart'
    Then    :   Tests Top right menus are working
    #------------ END test_b_topRightMenu(self):----------------------------

#--------------------------------------------------------------------------

    #--------------------------------------------------------------------
    # this test covers MAIN MENU
    # --> FURNITURE --> ART  --> JEWELRY & WATCHES --> FASHION --> 
                    --> INTERIORS --> NEWS & CUSTOM --> STYLES --> SALES
    #------------def test_c_mainMenu(self)::---------------------------    
    Scenario:   Hower over on menus 
    Given   :   On site user home page, after logging in
    When    :   on user home page, 
    And     :   Hover over 'FURNITURE' main menu and then sleep 1sec 
    And     :   Hover over 'Art' main menu and then sleep 1sec
    And     :   Hover over 'JEWELRY & WATCHES' main menu and then sleep 1sec
    And     :   Hover over 'FASHION' main menu and then sleep 1sec
    And     :   Hover over 'INTERIORS' main menu and then sleep 1sec
    And     :   Hover over 'NEWS & CUSTOM' main menu and then sleep 1sec
    And     :   Hover over 'STYLES' main menu and then sleep 1sec
    And     :   Hover over 'SALES' main menu and then sleep 1sec
    Then    :   AUTOMATE ON menus are working
    #------------ END test_c_mainMenu(self)::----------------------------

#--------------------------------------------------------------------------


    #--------------------------------------------------------------------
    # this test checks on BOTTOM MENUS 
    #------------test_d_bottom_menu(self):---------------------------    
    Scenario:   check BOTTOM MENUS 
    Given   :   On site user home page, after logging in
    When    :   on user home page, 
    And     :   Hover over 'Trade Program' bottom menu and put it in list var
    And     :   Hover over 'Seller Application' bottom menu and put it in list var
    And     :   Hover over 'Seller Login' bottom menu and put it in list var
    And     :   Hover over 'About us' bottom menu and put it in list var
    And     :   Hover over 'Support center' bottom menu and put it in list var
    And     :   Hover over 'Questions & Answers' bottom menu and put it in list var
    And     :   Hover over 'Press' bottom menu and put it in list var
    And     :   Hover over 'Careers' bottom menu and put it in list var
    And     :   Hover over '1stdibs Gallery' bottom menu and put it in list var
    And     :   Hover over 'Furniture' bottom menu and put it in list var
    And     :   Hover over 'Jewlery & watches' bottom menu and put it in list var
    And     :   Hover over 'Fine Art' bottom menu and put it in list var
    And     :   Hover over 'Fashion' bottom menu and put it in list var
    And     :   Hover over 'Creator' bottom menu and put it in list var
    And     :   Hover over 'Blog' bottom menu and put it in list var
    And     :   Hover over 'Magazine' bottom menu and put it in list var
    And     :   Select bottom menu in list var randomly
    And     :   Click on that menu & sleep 2sec
    And     :   Click on page back & sleep 2sec 
    Then    :   Check all bottom menus, and print randomly selected bottom menu
    #------------ END test_d_bottom_menu(self):----------------------------

#--------------------------------------------------------------------------
  
    
    # this test click on MAIN MENU "Furniture" and checks submenu links
    # also click randomly a submenu in Furniture's main menu 
    # and move to next product page
    #------------def test_e_furniture_menu(self):---------------------------    
    Scenario:   Hower over on main menu "Furniture" and hower on all its sub menus,  
    Given   :   On site user home page, after logging in
    When    :   on user home page, 
    And     :   Hover over 'Furniture' main menu and open it 
    And     :   Hover over on 'Furniture''s submenu & check all submenu are clicklbe(41 submenus) 
    And     :   put submenu in a list var
    And     :   Select a Furniture's submenu randomaly from list var
    And     :   Click on that submenu & sleep 1sec
    And     :   Empty List var 
    Then    :   Open 'Furniture' main menu and checks its submenu are clickable & randomly select 
                a submenu and click it
    #------------ END test_e_furniture_menu(self):----------------------------

#----------------------------------------------------------------------------


    # this test randomly select a product and click on that product--> move to next page
    #------------def test_f_select_product(self):---------------------------    
    Scenario:   Randomly select a product and click on it  
    Given   :   On product page, after clicking on main menus and select randomly it submenu
    When    :   Submenus' items put in a List variable, 
    And     :   choose a item randomly from List 
    And     :   click on that selected item    
    And     :   redirect to that selected item page
    And     :   sleep 2sec
    Then    :   randomly select a product & click it ---> redirect to specific page  
    #------------ END test_f_select_product(self):----------------------------




#----------------------------------------------------------------------------







    #--------------------------------------------------------------------
    # this test covers TOP RIGHT "My Account" MENU
    # My Account--> Account Information
    #           --> My Order
    #           --> My Conversations
    #           --> Logout
    #------------def test_w_myAccountMenu(self)::---------------------------    
    Scenario:   Hover over on Top right menu on 'My Account',open it and click on its submenus 
    Given   :   On site user home page, after logging in
    When    :   on user home page, 
    And     :   Hover over 'My Account', --> opens its submens 
    And     :   Click on 'Account Information' page redirects to Account information page & sleep 1see
    And     :   again Hover over 'My Account', --> opens its submens
    And     :   Click on 'My Orders' page redirects to My Orders page & sleep 1see
    And     :   again Hover over 'My Account', --> opens its submens
    And     :   Click on 'My Conversation' page redirects to My Conversation page & sleep 1see
    Then    :   Hover over 'My Account' menu and click on its submenu
    #------------ END test_w_myAccountMenu(self)::----------------------------

#--------------------------------------------------------------------------