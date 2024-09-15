# Personal Bowling Assistant
## Specification Deliverable
### Elevator Pitch
If you're like me and love the sport of bowling, you are well acquainted with the steep skill incline required to master the sport. What once was steady improvement through trial, error, and the full absorption of the fundamentals has come to a screeching halt; the immense knowledge of practical physics and inconsistent lane conditions act as a roadblock, suppressing your developmental journey. The Personal Bowling Assistant (or *PBA* for short) aims to alleviate the burden this barrier of entry leaves on the user. Users will be able to create an account with the system; in doing so, they will register their preferred bowling style and specific balls used, allowing the system to scrape stats from a reputable source to make accurate, personalized suggestions. Additionally, a user can host a game and invite other users to join. Upon updating individual gameplay data, each user will be able to see and interact with personal, real-time suggestions on their instance of the *PBA*. The Personal Bowling Assistant will be an instrumental aid in surpassing the demoralizing intricacies of bowling due to its unique analytical capabilities.
### Design
![*PBA* Design](https://github.com/user-attachments/assets/4f155638-69a1-42ad-bcc4-fab7e90cd5d2)
### Key Features
+ Secure login over HTTPS
+ Ability to input, save, and update important user info such as height, weight, average speed, bowling style, and balls used.
+ Ability to scrape reputable bowling sites and average bowling ball stats for accurate computations
+ Provide an additional UI for the host which will allow edits to the game immediately.
+ An interactive UI that allows the user to input their score, starting position, arrow thrown over, and contact point with each throw with real-time calculatory suggestions.
+ The ability to update, calculate, and display average stats
+ Additional features upon actualization
### Technologies
I am going to use the required technologies in the following ways.
+ **HTML** - Uses correct HTML structure for application. Five HTML pages. One for login, user, game creation, game admin, and game home
+ **CSS** - Application styling that looks good on different screen sizes, uses good whitespace, color choice, and contrast.
+ **React** - Provides login, use of React for routing and components, and more once development integration has been solidified.
+ **Service** - Backend service with endpoints for login and more once development integration has been solidified.
+ **DB/Login** - Store users and user info in database. Register and login users. Credentials securely stored in database. Can't interact with application unless authenticated.
+ **WebSocket** - a user can host a game, which allows other users to join and participate in real-time
