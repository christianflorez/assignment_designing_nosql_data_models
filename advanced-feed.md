## Activity Feed

You're building an activity feed for a social media site. The feed must display a chronological list of activities for the current user's friends. These activities could potentially be any action performed on the site including uploading a photo, changing their profile, friending another user, commenting, liking etc... Further, you only want to display activities for users that the current user interacts with frequently.

Nested Index List
Recent Actions Document:
* actionID: Integer
    * Must be at least 1 character
* friendID: Integer
    * Must be at least 1 character
* recentAction: String
    * Must be at least 5 characters
* timestamp: Datetime
    * Must be in MM/DD/YY - HH:MM:SS format

Index Table of primaryFriend: frequentFriendsArray relations
Frequent Friends:
* friendID: Integer

To display chronological activities, simply filter recent actions by frequent friends id