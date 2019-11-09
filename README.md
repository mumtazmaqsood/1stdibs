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