# Capstone

This app is focused on helping those who are new to technolpgy. This could range from help with wifi to fixing your font size. With each question a user types in it will try to find a tutorial that helps best. The user is also able to type in the company they're with and it will call their customer support number.


App evaluation:
Category: Education
Mobile: Website is view only, uses user input, mobile first experience.
Story: Allows users to get hep with their technology problems.
Market: Anyone that isn't skilled with technology can use this help. Sometimes someone might need help with fixing something on their phone or adjusting it to their liking but doesn't know where it's located.
Habit: Users can use this app whenever they need help. Throughout time it would be great to see the user getting used to their device by this app.
Scope: I believe this app won't be technically challenging.

Product Specs:
-Home screen with an input for users
-Multiple links highlighting the main idea
-Input for company which links to phone number
-Video screen of tutorial


Required Must-have:
[x] Input button
[] Phone call button
[] Links

Optional Nice-to-have:
-Share button
-Navigates you to which app to adjust your phone.


Screen Archetypes:
-Main Screen
  -User types in their question
  -User types in provider where a call button pops up
-Video screen
  -User sees which tutorial provides them with the most help.


Navigation:

Tab Navigation:
-Question search
-Button for tutorial

Flow Navigation:
-Question search
  -> Tutorial
-Provider input
  -> Home, phone call button will pop up
-Tutorials
  -> Tutorial link

Wireframes


<img width="536" alt="Screenshot 2024-04-15 at 2 27 08 PM" src="https://github.com/HalaEddouh/Capstone/assets/124421401/d647a177-ed46-4ffd-926d-9109c64bd8ff">




Checkpoint 1:
https://imgur.com/gallery/a4YLssn

So far i've completed the app evaluation which includes the navigation, screen archetypes and many more things. I've started my app and included a demo of it, which is linked above. So far my app has a search button and drop down for the providers.


Checkpoint 2:
https://imgur.com/gallery/cV6rgcF

Ran in to many errors and am still having to learn some things to add to my application. Still in progress...

Checkpoint 3:
https://imgur.com/gallery/KwLpBCS

FInal project. Still many things to improve on.


Schema
[This section will be completed in Unit 9]

Models

struct Video {
    let id: String
    let title: String
    let channelTitle: String
    let thumbnailURL: String
    var thumbnailImage: UIImage? // UIImage for thumbnail image, it could be optional if you download it later
}

Networking
[Add list of network requests by screen ]
[Create basic snippets for each Parse network request]
[OPTIONAL: List endpoints if using existing API such as Yelp]

Search Screen:
Request: Search YouTube videos based on user query.
Parameters:
q: Query string
part: Specifies the video resource parts that the API response will include.
type: Specifies the type of search resource to retrieve.

Video Selection Screen:
Request: Retrieve details of a specific YouTube video.
Parameters: id: The ID of the video.

Video Detail Screen:
Request: Retrieve video of a selected YouTube video.
Parameters: id: The ID of the selected video.
part: Specifies the video resource parts that the API response will include (e.g., snippet, statistics).
