# Bootcamp-PreWork
# Pre-work - *TodoAppDatabase*

**Name of your app** is an android app that allows building a todo list and basic todo items management functionality including adding new items, editing and deleting an existing item.

Submitted by: **Carolyn Sher-DeCusatis**

Time spent: **8** hours spent in total

## User Stories

The following **required** functionality is completed:

* [x] User can **successfully add and remove items** from the todo list
* [x] User can **tap a todo item in the list and bring up an edit screen for the todo item** and then have any changes to the text reflected in the todo list.
* [x] User can **persist todo items** and retrieve them properly on app restart

The following **optional** features are implemented:

* [x] Persist the todo items [into SQLite](http://guides.codepath.com/android/Persisting-Data-to-the-Device#sqlite) instead of a text file
* [ ] Improve style of the todo items in the list [using a custom adapter](http://guides.codepath.com/android/Using-an-ArrayAdapter-with-ListView)
* [ ] Add support for completion due dates for todo items (and display within listview item)
* [ ] Use a [DialogFragment](http://guides.codepath.com/android/Using-DialogFragment) instead of new Activity for editing items
* [ ] Add support for selecting the priority of each todo item (and display in listview item)
* [ ] Tweak the style improving the UI / UX, play with colors, images or backgrounds

The following **additional** features are implemented:

* [ ] List anything else that you can get done to improve the app functionality!

## Video Walkthrough 

Here's a walkthrough of implemented user stories:

<a href='http://decusatis.net/carolyn/DatabaseWalkThru2.mp4' title='Video Walkthrough'> Video Walkthrough of Project with Database</a>


## Project Analysis

As part of your pre-work submission, please reflect on the app and answer the following questions below:

**Question 1:** "What are your reactions to the Android app development platform so far? Compare and contrast Android's approach to layouts and user interfaces in past platforms you've used."

**Answer:** When I first started programming in Android five or six years ago, I used Eclipse, and it was pretty straightforward.  Now that Android Studio is the standard, there are many issues that I feel I need to improve on.  I have had to add memory to my computer, because 8 GB wasn't sufficient anymore.  I teach, but when I receive projects to review from my students, they often won't run due to gradle issues.  There was a memory management change between Lollipop and Marshmallow and I feel that I don't fully understand the implications of this. And when I design a screen, much of the time I have to do so manually in XML, because the drag and drop interface doesn't always create designs that display properly on phones.  Scene Builder with FXML seems to do a more consistant job than the XML editor in Android Studio. It seems the barrier to entry has gotten higher, and I need to work more consistently to vault over it. I want to understand it better, for my students, and for my research. 

**Question 2:** "Take a moment to reflect on the `ArrayAdapter` used in your pre-work. How would you describe an adapter in this context and what is its function in Android? Why do you think the adapter is important? Explain the purpose of the `convertView` in the `getView` method of the `ArrayAdapter`."

**Answer:** In my work so far, I use a standard ArrayAdapter to convert an ArrayList so it can be displayed ListView. As it states in the Android Developer's Guide, it's a bridge between the view and the underlying data, which is important because it links the backend to the users. In my application, the arraylist is populated from a database. It adds and removes items from the view, and is notified if the list is changed. 

The getView() method gets a View that displays the data at the specified positon of the data set. convertView is the old view in which to display the information. I don't really use it in my application- the information is simple enough that I just pass it between intents in the extras of the Bundle. But I suppose this reflection is here to prompt me to consider using it as I modify the application, and pass more complex information. 

## Notes

Must have mistakenly erased the constructing the ArrayList when cleaning up the app before quitting for the day-it started crashing when I opened it the next day. It took a little while to find the problem, since I didn't intend to do it! 

When adding the database things went relatively smoothly.  Followed http://www.vogella.com/tutorials/AndroidSQLite/article.html

## License

    Copyright [] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
