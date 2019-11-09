# stdibs
selenium + python testing www.stdibs.com

Implemented POM , CREATED SIX PAGES AND 23 TEST CASES AND GENERATED REPORTS, 
#UNITEST FRAME WORK USED 




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


    # this test covers TOP RIGHT MENU
    # My Account--> Notification --> order etc
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

