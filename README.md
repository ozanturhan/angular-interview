# Angular Project 

## Requirements
* Angular (Latest Version)
* NGXS
* RxJS

## Features to be Used
* Reactive Forms
* Lazy Loading Modules
* Unit Test With Jasmine (Jest is a big plus)
* Resolver


## General Descriptions

* A responsive design should be created.
* You can design the ui as you wish. 
* The users in users.json in the root directory should be shown hierarchically on the left side of the screen.
* Layout structure should be designed to be fixed on the left.
* Lazy load routing should be used.

## Screens

### Post List
<img src="mockups/post_list.png" height="400px">

* For each user selected from the hierarchy, the posts of the user should be taken through the user list API and kept on the state and listed on the screen.
* If there is a post list on state for the relevant user, api request should not be called again, the list should be filled by state.
* When mouse hovering over the lines, detail, edit and delete buttons should be displayed under the relevant line.
* When clicking Detail button post detail screen should be opened with choosen post id.
* When clicking Remove button related line should be removed without any api call. (it should be removed in the state).
* Must have ability to edit multiple lines.  
* When the save button is clicked, the api requests for each line must be made at the same time (parallel). After this process, the view mode should be returned and the values returned as a result of the operation should be displayed on the screen in view mode.
* A search input should be added to the screen on the client side and the search should be triggered when the number of letters exceeds 3.
* A select box should be placed to sort by id, title and body.
* If there is any line in edit mode, search and sort inputs should be disabled.

### Post Detail
<img src="mockups/post_detail.png" height="400px">

* When opening this screen, the post detail api should be called and the information on the screen should be shown with the values returned from this api.
* When the page is refreshed, there should be no errors in the working logic.

### Post Edit
<img src="mockups/post_edit.png" height="400px">

* With the edit button on the post detail page, you should switch to view mode.
* An alert should be issued when trying to refresh the page after making a change in the edit mode.
* If the page is refreshed without making changes, it must be opened in view mode.
* Remove action should delete the relevant post through state.

### Post Remove Confirmation
<img src="mockups/post_remove_confirmation.png" height="400px">

* When trying to delete the post, modal should be shown on the screen.
* This modal should be displayed on all screens where the remove action is called.