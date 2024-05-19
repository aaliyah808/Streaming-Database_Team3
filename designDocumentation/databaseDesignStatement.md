# Database Design Statement

## Purpose and Mission Statement

The purpose of our database is to maintain a music distribution and streaming platform’s data on the production and upload of digital audio files; users’ interaction, purchase, and downloading of digital audio files; and record engagement among users. The database keeps the purchase, download, like, and listen history of users and the accumulated income of labels. Data records related to social features and digital files are available to all users and labels who release music. Sensitive information related to invoice numbers in purchasing history and account registration is private to the users themselves. The labels who receive payment for transactions have access to purchase and sales data. 

## Business Problems Addressed

  * Allow users to freely listen to different genres of music and review their listening history
  * Allow users to find information about specific music, such as price and label
  * Allow users to create playlists containing different genres of music
  * Promote users to interact with other users by following and music by liking
  * Allow users to purchase music if they want to download and listen to the music offline
  * Allow users in certain specialties to release their music creations
  * Collect data on users' activity and music preferences to train the recommendation algorithm and formulate business strategies

## Business Rules

1. All users can listen to, like, purchase, and download zero to many tracks
2. All users can follow zero to many users
3. All users can participate in one or many musician activities.
4. Each track must involve one or many musician activities.
5. Each musician activity involves one musician's specialty
6. Users who have purchased a track/album can download it
7. Product as a superclass, has two subclasses: track and album.
8. All albums must have one to many tracks
9. One track must be in one and only one album
10. One playlist must have one to many tracks
11. One playlist cannot have repeated tracks
12. One playlist must be owned by one and only one user
13. One product must have one and only one label
14. One product must have one and only one listed price.
15. One purchase history must have one and only one invoice price (which is different from the product price)
16. One purchase history must belong to one and only one user
17. One purchase history must contain one and only one kind of product
18. One track must have one to many genres
