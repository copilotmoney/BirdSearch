# Bird Search Take Home Exercise

This is a take home exercise where we'll build an iOS App that displays common birds from Chile.

Your job is to take the following API and build an app that displays a list of birds along with
their image, and a search bar. Upon tapping on a row, a detail view controller should be presented
with the large version of the image.

When editing the search bar, the list of birds should be filtered to display birds where the name
(or part of it) matches the search text.

This shouldn't take you more than 3 hours to complete.

## Design Specs

Before starting this project, your interviewer will provide a Figma link that will contain the
design specs for the exercise. They should be followed as closely as possible. You will need to
create an account in order to view the specs, but it should be as easy as providing an email address
and clicking on the link on the confirmation email.

## API and data model

The API to use to display the birds is located in `https://aves.ninjas.cl/api/birds`. This API is
structured the following way:

```
[
    {
        "uid": "<Bird ID>",
        "name": {
            "spanish": "<Bird Name Spanish>",
            "english": "<Bird Name English>",
            "latin": "<Bird Name Latin>",
        },
        "images": {
            "thumb": "<Bird Thumb Image>",
            "full": "<Bird Full Image>"
        },
        "sort": <Bird Index>
    },
    ...
]
```

There are other fields available in the API, but they are not needed in the design spec. Feel free
to use the new async/await Swift APIs to download the data and handle asynchronous tasks (it should
be much easier).

## Project dependencies

External dependencies are allowed, feel free to use Swift Package Manager or Cocoapods dependencies.

## Delivery

Please clone this repository and create a new private Github repository under your account, giving
read access to the interviewer (or create a public repository if you want to, this is up to you).

Please also send an email to the interviewer letting them know that you've finished the exercise.

## Bonus points

* Make the presented image zoomable with a pinch gesture.
* Add pull to refresh to the bird list.
* Handle slow and failed downloads gracefully.

## Questions

Feel free to ask any questions to the interviewer throughout the process!