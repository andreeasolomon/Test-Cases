# Test-Cases
Test cases written in Qase. 

## Login eMAG

### Login with correct credentials

**Description**:
Check if the login works when a user enters the correct credentials.

**Steps to reproduce**:
1. Open emag.ro/user/login
2. Add correct username
3. Click "Continue" button
4. Enter correct password
5. Click "Login" button

**Expected result**:
User should be able to login and is redirected to his profile page.

**Test data**:
_user_: andreea
_password_: 123

**Pre-conditions**: User should have a valid account.

------------------------------------------

### Login with wrong credentials

**Description**:
Check if the login works when a user enters the wrong credentials.

**Steps to reproduce**:
1. Open emag.ro/user/login
2. Add Add wrong username
3. Click "Continue" button
4. Enter wrong password
5. Click "Login" button

**Expected result**:
User should not be able to successfully login with the wrong credentials.

**Test data**:
_user_: any letter, number or symbol,
_password_: any any letter, number or symbol

------------------------------------------

### No credentials login

**Description**:
Check if the login works when a user does not enter the credentials.

**Steps to reproduce**:
1. Open emag.ro/user/login
2. Leave the username box empty
3. Click "Continue" button
4. Leave the password box empty
5. Click "Login" button

**Expected result**:
An error should appear in which the user is informed that the account cannot be accessed if the fields "Username" and "Password" are not filled.

-----------------------------------------

### Wrong username and correct password

**Description**:
Check if the login works when a user enters the wrong username and the correct password.

**Steps to reproduce**:
1. Open emag.ro/user/login
2. Add wrong username
3. Click "Continue" button
4. Enter correct password
5. Click "Login" button

**Expected result**:
User should not be able to successfully login into his account.

**Test data**:
_user_: any username,
_password_: 123 (must be correct)

---------------------------------------

### Correct username and wrong password

**Description**:
Check if the login works when a user enters the correct username and the wrong password.

**Steps to reproduce**:
1. Open emag.ro/user/login
2. Add correct username
3. Click "Continue" button
4. Enter wrong password
5. Click "Login" button

**Expected result**:
User should not be able to successfully login into his account.

**Test data**:
_user_: any username (must be correct),
_password_: 123

---------------------------------------

## Search eMAG

### Zero results for non-existent items

**Description**:
Check if the search functionality has zero results when the user searches for non-existent items.

**Steps to reproduce**:
1. Open emag.ro
2. Click on "Search"
3. Write any word, e. g. "yuhu"
4. Press enter

**Expected result**:
User should receive zero results when looking for items that do not exist.

-----------------------------------------

### Successfully searching on eMAG

**Description**:
Check if the search functionality works correctly by showing the expected results.

**Steps to reproduce**:
1. Open emag.ro
2. Click on "Search"
3. Write any word, e. g. "bed"
4. Press enter

**Expected result**:
User should be able to see multiple results about the searched item.

--------------------------------------------

### Autocompletion of search functionality

**Description**:
Check if the search functionality autocompletes while the user writes in the "search" box.

**Steps to reproduce**:
1. Open emag.ro
2. Click on "Search"
3. Write any word, but not completed, e. g. "ov"
4. See if additional letters appear after the first two letters, e. g. "en"

**Expected result**:
User should be able to see if the word will be autocompleted.
