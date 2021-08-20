# MentGo-App

## Overview
In recent years, society has come to acknowledge the growing concern for mental health in various situations. Most notably is the mental health statements posed by atheletes including Simone Biles in this year's recent Olympics as well as Paul George in the NBA Bubble during the COVID-19 lockdown. However, mental health branches off even further than that into many other aspects of society. Take, for instance, students. In the years of high school and college, students face an overwhelming amount of pressure from external sources whether it be related to getting into a "good" college, achieveing the best grades possible, securing internships, etc. Seeing the range of mental health concerns popping up, it is imperative for there to be an avenue that can, in some way, push to have people seek help in an efficient manner.

## Purpose
Within the range of mental health, there are many avenues that can assist. There are various hotlines all across the internet hosted by specific organizations that can assist. There are also ways to cope with mental health in videos that can be found on online platforms such as Youtube. However, information is scattered. In a time of need where a person must dial a hotline or quickly access a form of relief, it is grueling to have to perform an internet search first and then look for a specific search result. This is where MentGo comes in to be an intermediary, made with an application development software known as Flutter in the Dart programming language. The purpose of MentGo is consolidate mental health resources that provide ease of access, allowing all information needed to be present. A key feature is having all hotlines on display as a "home" page so as soon as the user loads into the application, a simple click of button proceeds to a call that can be made since all the numbers are stored. The following information will demonstrate the features of MentGo as well as the process of creation.

## Base UI
To begin the design process, I was able to create a base of the UI on the load screen. Before this load screen, there is also an initial splash screen as an introduction which lasts for approximately 3 seconds. The following visual shows the homescreen. 
![Screenshot_1629388711](https://user-images.githubusercontent.com/66923911/130102805-12ee4285-5bc0-4a60-add9-f06b663222ae.png)

The flow of the design is two different pages that the user can access: the maps page which displays a map with nearby mental health clinic locations, and then a calls/tips page with the main quick call page as well as additional personal tips including breathing exercises and statistics.

## Calls & Tips
The next portion of this flow will be a depiction of the different screen. Looking first at the calls & tips page, the following is the initial screen the user is greeted with:
![Screenshot_1629388726](https://user-images.githubusercontent.com/66923911/130113282-ab26d3e5-ec55-4b1f-8263-989796d8c289.png)

The above image displays the main call screen with various elements. In an emergency situation, an individual can click the EMERGENCY CALL button and be redirected to a pre-filled call screen for the Suicide Prevention Hotline. In addition to this, there is an EMERGENCY TEXT screen available to individuals that may not want to have a verbal conversation and are much more comfortable sending text messages. Below this header is the call buttons. The buttons are organized based on the mental health category (calls and buttons will continue to be added as more are made available). Clicking these buttons redirects the user again to a call screen with the pre-set number.

The next tips screen is shown below:
![Screenshot_1629388733](https://user-images.githubusercontent.com/66923911/130285620-5c77ed59-8847-4209-a9ef-5b86712e4c36.png)

The above tips screen has the main display as being a circular wheel to showcase all the important aspects of mental health. Currently, the main feature is a list of Youtube videos below that disply certain breathing exercises. There are a variety of breathing exercises and those will eventually be supplemented with statistics related to mental health as well as words of wisdom from those that have battled through those situations.

## Map and Locations
A primary feature of this MentGo application is the map page that shows off the nearby locations that match the query "mental" in the Google Maps API which returns a list of places that are then displayed in cards as shown below:
![Screenshot_1629484671](https://user-images.githubusercontent.com/66923911/130287685-93c76ffc-f57a-411f-90d9-cbde9fbfb377.png)

The above image shows that the default location given for an Android Emulator in Flutter is the Googleplex. Near this location, there are markers that show the nearby clinics and a card view below the map. In the card view, a rating and address is given to the user along with the name of the place. To the right of the name is a button that shows directions to the selected place by launching Google Maps. Lastly, there is a small number that represents the distance in miles that a place is to the user currently. A distance of 0 miles means that the place is less than half a mile from the user since the final result is rounded.
