# startup

# cedhmeta.com | The Global cEDH Data Tracker

## Elevator Pitch
Track your cEDH games and get accurate data on your performances. In just a few easy clicks, you can get state-of-the-art projections on what to change to be a better cEDH pilot and deckbuilder. The cEDH Meta Project only accepts verified data where all four players have registered accounts, letting you trust the numbers and feel good about how you're matching up against other players. Unlike outdated programs, cEDH Meta uses an alternate points system, known as Prowess, that better reflects your individual performance, taking into account things like turn order and the overall skill-level of the people you were playing against So while winning is still the most important outcome, there is a lot more to a cEDH game than just that.

## Design

![alt text](https://github.com/JayWheels/startup/blob/main/cedhmeta.png "cedhmeta.com")

![alt text](https://github.com/JayWheels/startup/blob/main/cedhmeta2.png "cedhmeta.com")

## Key Features

- Secure login over HTTPS
- Ability to log regularly played commanders for quick selection
- Ability to enter game results, including a relative date
- Game logs are sent to the other three players for verification
- Points and point changes displayed in real time based on game results
- Results are stored
- Player can view result history
- Admin can delete logs and remove them from data pools
- Player can view their standing compared to other players

## Technologies

- HTML - HTML structure will be used for this application, including multiple HTML pages. Main page for current leaderboards, a history page for past matches, a profile page, etc.
- CSS - Application styling will look good and have the modern reactivity, coloring, and feel to the user experience
- JavaScript - Login, opening submission windows, allowing for manipulation of visible data
- Service - Backend endpoints for:
  - login
  - submitting game logs
  - retrieving a list of players to be narrowed down for submission
- DB - Store users, game logs, prowess points, commanders and more
- Login - Register and login users. Credentials will be stores. Can't submit unless the user is authentificated and all four other users are authentificated
- WebSocket - When games are submitted, each involved user is sent a notification about the game submission so it can be verfified. Once verified, the results are then posted to the entire website.
- Application will be ported for React web framework (I am still learning what this means)

