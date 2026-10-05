# Topic
Our app, Naviscape, is a maps-based web application focused around points of interest and collaboration. It aims to incorporate groups and social planning with an online, interactive points-of-interest navigator. We list out POIs such as attractions, food, parks, shopping, etc. to users based on selected locations and allow them to interact with these places, in ways like "favourite-ing", reviewing and pinning / highlighting. The social aspect comes with being able to friend other users and creating groups, in which people can pin or highlight locations that will show up to other people in the group. This helps increase group collaboration for things such as vacation planning, club/group field trips, and formal dinners, and keeps everyone in the group on the same page.  Inferentially, our app's target audience is a wide range of people; anyone who utilizes smart technology in their day-to-day, and is often involved in social (or any kind of group) events.

## Data Source
Our primary data source is [Geoapify](https://www.geoapify.com/). From here we will get data about locations. Our secondary data source is Google's [Places API](https://developers.google.com/maps/documentation/places/web-service/overview), from which we will only request photos of locations to display on our website.

Sample data shape of Geoapify:
```
{
  "results": [
    {
      "name": "Caluire-et-Cuire",
      "city": "Caluire-et-Cuire",
      "state": "Auvergne-Rhône-Alpes",
      "postcode": "69300",
      "country": "France",
      "country_code": "fr",
      "formatted": "Caluire-et-Cuire, ARA, France",
      "lat": 45.7969952,
      "lon": 4.8423304,
      "result_type": "city",
      "place_id": "51d6b441dc8b5e134059d4884ff003e64640f00101f9017162010000000000c0020892031043616c756972652d65742d4375697265"
    }
  ]
}

```

Sample data shape of Google Places API's Place Photos:
```
    ...
    "photos" : [
      {
        "name": "places/ChIJ2fzCmcW7j4AR2JzfXBBoh6E/photos/AUacShh3_Dd8yvV2JZMtNjjbbSbFhSv-0VmUN-uasQ2Oj00XB63irPTks0-A_1rMNfdTunoOVZfVOExRRBNrupUf8TY4Kw5iQNQgf2rwcaM8hXNQg7KDyvMR5B-HzoCE1mwy2ba9yxvmtiJrdV-xBgO8c5iJL65BCd0slyI1",
        "widthPx": 6000,
        "heightPx": 4000,
        "authorAttributions": [
          {
            "displayName": "John Smith",
            "uri": "//maps.google.com/maps/contrib/101563",
            "photoUri": "//lh3.googleusercontent.com/a-/AD_cFT-b=s100-p-k-no-mo"
          }
        ]
      },
    ...
```

## Comparators
Two of our biggest comparators are Google Maps and Snapchat's Snap Map. Google Maps is obviously unbeatable in general navigation, and Snap Map is similar in the fact that it displays a navigable globe map but it includes being able to see your friends' locations (who opt to do so). Naviscape differs in actually being able to highlight and share locations with friends in real time.

## Scaled Feature List
| Feature               | Purpose                                                            | Owner        |
|-----------------------|--------------------------------------------------------------------|--------------|
| User Profiles Page    | Displays a webpage of an individual user's profile                 | Shan Jeofry  |
| Login Page            | A login page including "remember me" and "forgot password" options | Abbas Syed   |
| HTML / CSS Structure  | Base framework and styling for entire website                      | Ethan Jallim |
| Searching / Filtering | Search / filter / sort POIs                                        | Hasan Nawaz  |
