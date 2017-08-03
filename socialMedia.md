# Needs

* Activities
  * Action Type
  * Time
  * User

* Users
  * Friends (people they interact with?)

## Model

```javascript

User: {
  Activities: {
    Date: [notificationId, notificationId,...],
    Date: [notificationId, notificationId,...],
    Date: [notificationId, notificationId,...]
  },
  Friends: [userId, userId, userId],
  Profile: {
    [personal details]
  }
}

activityNotifications {
  notificationId: {
    actionName: String,
    actionTime: Date,
    actionUser: userID,
    actionLink: String,
    actionType: [action document type],
    actionId: actionId
  }
}

likes: {
  likeID: {
    literallyAnything: {}
  }
}

comments: {
  commentID: {
    literallyAnything: {}
  }
}

photos: {
  photoId: {
    literallyAnything: {}
  }
}



```
