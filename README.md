Codepath Group Project - README Template
===

# FoodShare

## Table of Contents
1. [Overview](#Overview)
1. [Product Spec](#Product-Spec)
1. [Wireframes](#Wireframes)
2. [Schema](#Schema)

## Overview
### Description
The FoodShare app is an app to help nearby on-campus students share excess food with each other. They can post excess food that they have and request food from others on-campus. If someone has something they would like to share, they can private message the student and collaborate on when and where to meet up. This app is meant to help students get to know their neighbors and to reduce food waste on-campus.

### App Evaluation

- **Category:** Food and Lifestyle
- **Mobile:** iOS app
- **Story:** Connects users with neighbors in order to share excess food. The user can message other students to request/offer their excess food
- **Market:** On-campus college students
- **Habit:** This app can be used whenever they are cooking food, probably using the app every week or more
- **Scope:** All campus students, apartment residents, condominiums

## Product Spec

### 1. User Stories (Required and Optional)

**Required Must-have Stories**

* Users can create an account
* Users can post that they have excess food
* Users can directly message each other to request/offer food
* Users can scroll through lists of existing offers
* Users can close their post when it is accepted
* Users can log out through a profile page

**Optional Nice-to-have Stories**

* Nice to be able to friend other users so they can appear first
* Nice to have categories for popular items
* Nice to restrict access to .edu emails only
* Nice to search offers based on proximity or type

### 2. Screen Archetypes

* Login Screen
* Register Screen
   * Users can create an account
* Scroll Screen
   * Users can scroll through lists of existing posts
* Creation Screen
   * Users can post that they have excess food
* Messaging Screen
   * Users can directly message each other to request/offer food
   * Users can close their post when it is accepted

### 3. Navigation

**Tab Navigation** (Tab to Screen)

* Scroll Screen
* Messaging Screen
* Creation Screen
* Settings Screen

**Flow Navigation** (Screen to Screen)

* Forced Login -> Account creation if no login is available
* Post selection -> Messaging screen to accept the offer
* Messaging selection -> Individual messaging chats
* Logout -> Login screen

## Wireframes
[Add picture of your hand sketched wireframes in this section]
<img src="YOUR_WIREFRAME_IMAGE_URL" width=600>

### [BONUS] Digital Wireframes & Mockups

### [BONUS] Interactive Prototype

## Schema 

### Models
Post

| Property | Type | Description |
| -------- | ---- | ----------- |
| objectId | String | unique id for the user post |
| imageFood | file | food image that user posts |
| description | String | post description that user posts |
| createdAt | DateTime | date when post is created |
| author | Pointed to User | author of post |
| authorImage | file | author's profile picture |

### Networking
- [Add list of network requests by screen ]
- [Create basic snippets for each Parse network request]
- [OPTIONAL: List endpoints if using existing API such as Yelp]