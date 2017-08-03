# Needs
* Login
* Profile information and settings
  * birthday -> toggleable visiblilty
  * gender -> toggleable visiblilty
  * phone number -> toggleable visiblilty
  * location -> toggleable visiblilty
    * city
    * state
    * country
  * profile

## Model

```javascript
Person: {
  loggedIn: boolean,
  bio: string,
  profile: {
    birthday: {
      value: stringified Date,
      visible: boolean
    },
    gender: {
      value: string,
      visible: boolean
    },
    phoneNumber: {
      value: number,
      visible: boolean
    },
    location: {
      value: {
        city: string,
        state: string,
        country: string
      },
      visible: boolean
    }
  }
}
```
