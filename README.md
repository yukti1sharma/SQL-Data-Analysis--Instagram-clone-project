# SQL-Data-Analysis--Instagram-clone-project

This project is a clone of Instagram, implementing key features such as user profiles, photo uploads, comments, likes, and follows. The purpose of this clone is to practice and demonstrate database design, relational database management, and basic web application functionality using SQL.

## Features
User Management: Create and manage user profiles.
Photo Uploads: Users can upload and view photos.
Comments: Users can comment on photos.
Likes: Users can like photos.
Follow System: Users can follow and unfollow each other.
Tags: Users can add tags to photos for better categorization.


## Database Schema

### Users
Stores user information.

id: Unique identifier for each user (Primary Key)
username: Username of the user
created_at: Timestamp of when the user was created


### Photos
Stores information about user-uploaded photos.

id: Unique identifier for each photo (Primary Key)
image_url: URL of the photo
user_id: ID of the user who uploaded the photo (Foreign Key)
created_at: Timestamp of when the photo was uploaded


### Comments
Stores comments made on photos.

id: Unique identifier for each comment (Primary Key)
comment_text: Text of the comment
user_id: ID of the user who made the comment (Foreign Key)
photo_id: ID of the photo being commented on (Foreign Key)
created_at: Timestamp of when the comment was made


### Likes
Stores likes given to photos.

user_id: ID of the user who liked the photo (Foreign Key)
photo_id: ID of the photo that was liked (Foreign Key)
created_at: Timestamp of when the like was given
Primary Key: Composite of user_id and photo_id


### Follows
Stores user follow relationships.

follower_id: ID of the user who is following (Foreign Key)
followee_id: ID of the user being followed (Foreign Key)
created_at: Timestamp of when the follow action occurred
Primary Key: Composite of follower_id and followee_id


### Tags
Stores tags for categorizing photos.

id: Unique identifier for each tag (Primary Key)
tag_name: Name of the tag
created_at: Timestamp of when the tag was created


### Photo Tags
Junction table for associating photos with tags.

photo_id: ID of the photo (Foreign Key)
tag_id: ID of the tag (Foreign Key)
Primary Key: Composite of photo_id and tag_id






### I have run several queries for knowing the tables more! 
