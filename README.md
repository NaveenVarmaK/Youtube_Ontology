# YouTube Ontology

## Introduction

This is a collaborative project to develop an ontology for the YouTube social network platform. This project aims to model the YouTube social network using an ontology from a course work on **Knowledge Representation and Reasoning** which is one of the modules of the Artificial Intelligence Challenge at École des mines de Saint-Étienne. The ontology describes various entities such as users, videos, channels, comments, categories, and activities, along with their relationships and properties.

## Contributors

- [Naveen Varma Kalid](https://github.com/NaveenVarmaK)
- [Adeuyi Anjolaoluwa Joshua](https://github.com/anjola-adeuyi)
- [Tetteh Rockson](https://github.com/Rockson95)
- [Francis Alex Nwagbo](https://github.com/Franlexa)

## Modeling the YouTube Social Network

The team has worked on modeling the following key components of the YouTube social network:

## Classes

- **User**: Represents a user of the YouTube platform.
  - **Subclasses**
    - RegisteredUser
    - GuestUser
- **Video**: Represents a video uploaded to the YouTube platform.
  - **Subclasses**
    - Vlog
    - MusicVideo
- **Channel**: Represents a channel on YouTube.
  - **Subclasses**
    - None
- **Comment**: Represents a comment left by a user on a video.
  - **Subclasses**
    - None
- **Category**: Represents a category or genre classification for videos.
  - **Subclasses**
    - Music
    - Gaming
    - Education
    - Entertainment
- **Playlist:** Represents a collection of ordered videos curated by a user or channel.
  - **Subclasses**
    - None
- **Activity**: Represents various actions performed by users on the platform.
  - **Subclasses**
    - Upload
    - CommentOn
    - Like
    - Dislike
    - Subscribe
    - Share
- And more...

## Relationships

- **Uploads (User, Video)**: Defines the relationship between a user and a video.
  - **Example:** User A uploads Video X.
- **Creates (User, Channel)**: Indicates that a user has created a channel.
  - **Example:** User B creates Channel Y.
- **Includes (Channel, Video)**: Specifies that a video is included in a channel's library.
  - **Example:** Channel Y includes Video Z.
- **Contains (Playlist, Video):** Indicates that a video is contained within a playlist created by a user or channel.
  - **Example:** Playlist P contains Video Q.
- **Comments on (User, Video)**: Represents a user leaving a comment on a video.
  - **Example:** User C comments on Video X.
- **Categorized under (Video, Category):** Specifies the category classification of a video on the platform.
  - **Example:** Video X is categorized under the Music category.
- **Subscribes (User, Channel):** Indicates that a user has subscribed to a channel to receive updates on its content.
  - **Example:** User D subscribes to Channel Y.
- **Likes/Dislikes (User, Video/Comment):** Represents a user expressing their opinion by liking or disliking a video or comment.
  - **Example:** User E likes Video X.
- **Shares (User, Video):** Indicates that a user has shared a video on social media or other platforms.
  - **Example:** User F shares Video X.
- And more...

## Data Properties

- **userID**: Represents the unique identifier of a user.
  - Example: User A has userID "123456789".
- **channelID**: Represents the unique identifier of a channel.
  - Example: Channel X has channelID "987654321".
- **videoID**: Represents the unique identifier of a video.
  - Example: Video Y has videoID "567890123".
- commentID: Represents the unique identifier of a comment on the YouTube platform.
  - Example: Comment Z has commentID "345678901".
- categoryID: Represents the unique identifier of a category or genre classification on the YouTube platform.
  - Example: Category Music has categoryID "123". #anjo can you confirm this, i am not sure about this
- playlistID: Represents the unique identifier of a playlist on the YouTube platform.
  - Example: Playlist P has playlistID "456".
- **timestamp**: Represents the date and time when an action occurs.
  - Example: Video X was uploaded at timestamp "2024-04-15T15:00:00".
- viewCount: Represents the number of views a video has received on the YouTube platform.
  - Example: Video Y has a viewCount of 1000.
- likeCount: Represents the number of likes a video or comment has received on the YouTube platform.
  - Example: Video Z has a likeCount of 500.
- dislikeCount: Represents the number of dislikes a video or comment has received on the YouTube platform.
  - Example: Video W has a dislikeCount of 100.
- subscriberCount: Represents the number of subscribers a channel has on the YouTube platform.
  - Example: Channel V has a subscriberCount of 5000.
- duration: Represents the duration or length of a video on the YouTube platform.
  - Example: Video U has a duration of "00:10:30" (10 minutes and 30 seconds).
- And more...

## Optional Logs

- Viewing Activity
- Liking Activity
- Commenting Activity
- Sharing Activity
- Subscription Activity
- Live Stream Activity
- Disliking Activity
- Playlist Creation Activity
- Channel Creation Activity
- Video Upload Activity
- And more...

## Screenshots
![Screenshot 2024-04-13 192459](https://github.com/NaveenVarmaK/Youtube_Ontology/assets/64104378/b08c3bff-d820-4883-819c-058fa4abaa0b)![Screenshot 2024-04-13 192528](https://github.com/NaveenVarmaK/Youtube_Ontology/assets/64104378/6523c814-f75f-4d06-917d-37c99a64dea0)


## Examples

An examples of how entities, relationships, and properties are used in our youtube ontology. [Youtube_Ontology.ttl](https://github.com/NaveenVarmaK/Youtube_Ontology/blob/main/Youtube_Ontology.ttl)

## Usage

The YouTube Ontology can be used to integrate and leverage the knowledge model in various applications and systems related to the YouTube platform. This includes, but is not limited to:

- Developing intelligent video search and recommendation systems for YouTube content.
- Analyzing user behavior and engagement patterns on the platform.
- Enhancing content moderation and community management capabilities.
- Enabling advanced analytics and business intelligence for YouTube creators and platform owners.
- Developers can use the ontology to enrich metadata associated with YouTube videos, channels, and user interactions, enabling more intelligent and context-aware applications.
- Integrating the ontology with other data sources to create a comprehensive knowledge graph for the YouTube ecosystem.

To use the ontology, you can import the [Youtube_Ontology.ttl](https://github.com/NaveenVarmaK/Youtube_Ontology/blob/main/Youtube_Ontology.ttl) file into your preferred ontology management tool, such as Protégé. From there, you can explore the ontology structure, query the knowledge base, and integrate it into your applications.

Protégé's functionalities include:

- **Class Creation and Hierarchy Management:** We used Protégé to define classes like `User`, `Video`, `Channel`, and establish relationships between them (e.g., `User` uploads `Video`).
- **Property Definition:** Properties like `hasCategory`, `likeCount`, and `duration` were created within Protégé to specify characteristics of entities.
- **Reasoning and Inconsistency Detection:** Protégé's reasoning capabilities helped ensure the consistency of the ontology by identifying logical inconsistencies within the defined classes, relationships, and axioms.

**Additional Tools and Languages**
Beyond Protégé, other tools and languages can be employed to work with this ontology:

- **OWL (Web Ontology Language):** This standard ontology language was used to represent the YouTube Ontology's entities, relationships, and properties. OWL allows for machine-readable interpretation of the ontology's structure and semantics.
- **RDF (Resource Description Framework):** RDF serves as the foundation for expressing information in the ontology. It provides a framework for representing entities (resources), their properties, and the relationships linking them.

## Acknowledgments

We would like to to express our gratitude and acknowledge our professor, Professor Antoine Zimmermann, who is also one of the authors of the book **"KNOWLEDGE GRAPHS"** that we used for the course. Professor Zimmermann's research interests are related to the Semantic Web, more specifically on knowledge representation, knowledge engineering, reasoning, data management, and context on the Web. You can find more details about his work and research at https://www.emse.fr/~zimmermann/.

We would also like to thank the team members - [Adeuyi Anjolaoluwa Joshua](https://github.com/anjola-adeuyi), [Naveen Varma Kalid](https://github.com/NaveenVarmaK), [Tetteh Rockson](https://github.com/Rockson95), and [Francis Alex Nwagbo](https://github.com/Franlexa) - for their collaborative efforts and contributions to this project.
