---
layout: essay
type: essay
title: Botaniary App Proposal
date: 2016-10-22
labels:
  - Meteor
  - Botany
  - Hiking
  - App Development
---
Authors: Bill Mullen, Nathan Nahina, Matthew Schultz

## Overview


### The problem

There are a lot of plants out there on the University of Hawaii campus. However these plants are not always conveniently labeled. There is a significant lack of local plant identification apps out there and carrying around a plant field guide is not always convenient.
<ul>
<li>What if someone sees a plant but doesn’t have a field guide handy?</li>
<li>And what about those plants that are on campus that people hear about, but have never quite been able to find?</li>
<li>What about people interested in the practical uses of plants on campus as food, medicine, or other useful materials?</li>
<li>What about people who are keeping track of the health of plants and if certain ones have been damaged or removed?</li>
<li>What if one would want to know which plants are endemic to the islands?</li>
<li>What if someone would like to know the Hawaiian names of these plants?</li>
</ul>

### The Solution

Botaniary would be a fun, educational way for anyone with a myuh account to learn more about plants around the UH Manoa campus.

Botaniary’s base functionality would be a plant field guide and map, integrating the [map and underlying dataset on the landscaping section of the manoa.hawaii.edu website.](http://manoa.hawaii.edu/landscaping/plantmap.php) and other UH Manoa resources such as the [Manoa Campus Plants page](http://www.botany.hawaii.edu/faculty/carr/160webindex.htm)

Each plant would be tied to a pin/location on the map. Using google’s location api, the app would be able to do basic authentication to check if a user is near a plant. After authentication is established, a user would receive points and possibly achievements for walking to plants and verifying their condition and status.

Botaniary’s strength would be in crowdsourcing the identification and cataloguing of unknown plants and updating the status of . The point and achievement system would help keep users engaged and more involved and educated about nature.

Botaniary’s plant index would have options for filtering out based on attributes of plants; for example, if a user would like to view only plants native to Hawai’i, they would be able to by simply checking a box.

Users would also have the option to take a picture of previously unidentified plants and make dropdown selections about the appearance of the plants (leaves, flowers, colors, size, etc).


## Mockup page ideas

<ul>
<li>Public landing page displaying a map of the campus</li>
<li>Login page</li>
<li>User home page</li>
<li>User profile page</li>
<li>Plant index (‘botanodex’) page</li>
<li>Individual plant species page</li>
<li>Specific plant profile page (1 for each plant/tree/etc)</li>
<li>List of saved plant profiles for each user</li>
<li>Plant identification helper form</li>
<li>Admin home page</li>
<li>Top scores page</li>
<li>Menu page</li>
</uL>

## Use case ideas
<ul>
<li>New user goes to landing page, logs in, redirected to landing page for logged in users, user keeps map open to find a plant on campus, user receives points when they are in close range of the plant, user selects the plant on the map and navigates to the plant’s profile page, updating the status of the plant.</li>
<li>User has planted native plants near campus, to replace non-native invaders. User logs in to app, pulls up his own list of plant profiles, selects a specific plant profile from the list and walks to that plant. For newly planted plants, user may mark down when the plant has been watered, and other care details, and update the plant’s condition. User has option to make plant profile private or public (thereby inviting other users to check in on the plant).</li>
<li>User sees plant they don’t recognize, logs in to app. User navigates to plant identification, takes photograph of plant they don’t recognize, answers questions about plant features in flowchart-based format to identify plant, is presented with a picture of the identified plant (based on the features the user identifies) alongside the picture they took.</li>
<li>Admin goes to landing page, logs in, redirected to admin home page, views verification alerts, approves or denies user submitted entries to receive verified status in the index, navigates to index page, and adds new species and specific plants.</li>
</ul>

## Beyond the basics
<ul>
<li>Game elements (art/animation and map traversal)</li>
<li>Advanced filtering (i.e. Native, medicinal uses, edible, poisonous)</li>
<li>"Smart" automated plant identification from photos (Long term implementation. Possible graduate student project)</li>
<li>“Hike” feature - a user creates a routed hike, using a map tool to string together a walking route between a series of interesting plants. A common use would be to note periodic plant stops along one of the Manoa valley trails. Other users can select a hiking route, and mark off plants as they reach them.</li>
<li>Social features - chat, messaging, and adding friends.</li>
</ul>
