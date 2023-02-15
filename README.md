# Webmaster Hackathon

## Prototyping
## [Page Design & Flow](https://indiana-my.sharepoint.com/:p:/g/personal/gtnguyen_iu_edu/EXiy6fiQHO5Kk-9V8cNp_3sBMFEhdBp_koodIPwh8Hpe1A?e=6vHVMn)
## [Database Structure](https://github.com/alexbrahos/Webmaster_Hackathon/blob/main/erd.jpg)
### COLLABORATERS❗️❗️
Notes on testing:
Clone the repository / download the zip. Then, open "index.html" to experience a static version of the website. 

## Documentation 
### Summary
*Alpha Arcade* is a web application that allows for the user to play games. Users may want to login to keep log of their money. The money is used to buy and unlock more games. 
<br>
The games avaliable are:
1. Tap (free)
2. Rock, Paper, Scissors
3. Tic-Tac-Toe

### User Cases
There is only one type of user—the players. Players may want to create an account, as an account will ensure that in-game currency and games bought will be maintained outside of page refreshment. 

### Data Structure
To keep user login and accredited information persistent, cookies are used. All user information is appropriately stored in a relational database of four tables. 
<br>
[ERD](https://github.com/alexbrahos/Webmaster_Hackathon/blob/main/erd.jpg)

### Flow 
#### Login 
<br>1.1 Has an Account
<br>1.1.1 Correct credentials 
<br>1.1.1.1 Successfully logged in
<br>1.1.1.1.1 Redirected to 2.1
<br>1.1.2 Incorrect credentials 
<br>1.1.2.1 Redirected to 1.1
#### Main
<br>2.1 Library
<br>2.1.1 Select a game
<br>2.1.1.1 Redirected to GAME
<br>2.2 Store
<br>2.2.1 Redirected to STORE
<br>2.3 Profile
<br> Redirected to PROFILE
#### Playing a Game 
<br>3.1 Game loads 
<br>3.1.1 User plays the game 
<br>3.1.1.1 User wins
<br>3.1.1.1.1 User wins in-game currency 
<br>3.1.1.1.1.1 User may replay or return home
<br>3.1.1.1.1.1.1 User returns home
<br>3.1.1.1.1.1.1.1 Redirected to 2.1
<br>3.1.1.1.1.1.2 User replays game
<br>3.1.1.1.1.1.2.1 Redirected to 3.1
<br>3.1.1.2 User loses
<br>3.1.1.2.1 User wins no in-game currency
<br>3.1.1.2.1.1 User may replay or return home 
<br>3.1.1.2.1.1.1 User returns home
<br>3.1.1.2.1.1.1.1 Redirected to 2.1
<br>3.1.1.2.1.1.2 User replays hame
<br>3.1.1.2.1.1.2.1 Redirected to 3.1
#### Store
<br>4.1 Store loads
<br>4.1.1 User selects a game
<br>4.1.1.1 User purchases game 
<br>4.1.1.1.1 User has enough in-game currency
<br>4.1.1.1.1.1 Game permission is unlocked
<br>4.1.1.1.1.1.1 Redirected to 4.1
<br>4.1.1.1.2 User does not have enough in-game currency
<br>4.1.1.1.2.1 Redirected to 4.1
#### Profile 
<br>5.1 Profile loads
<br>5.1.1 User uploads image 
<br>5.1.1.1 Image is successfully uploaded 
<br>5.1.1.1.1 Profile picture is changed 
<br>5.1.1.2 Image is not successfully uploaded 
<br>5.1.1.2.1 Profile picture is unchanged
