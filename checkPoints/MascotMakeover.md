{% include "../includes/header.md" %}

<!-- @TODO ATTENTION: DEVELOPER, 

Checkpoint are test of what the student has learned in the past pre-homeworks and class. It should be started in the class just before it is due and takes the place of a project that would have been created during that week. 

1) FIND/REPLACE ProjectTitle to change titles in all sections
2) SEE EXAMPLE RUBRIC at bottom of file
3) If you need to create a repo for the student to clone:
  * Create the repo in the AustinCodingAcademy gitHub account and,
  * use the naming " NG421_W7D1_QuizAPI "

-->

# CheckPoint 1 - ProjectTitle

## ProjectTitle Overview

<!-- EXAMPLE OVERVIEW: Over the last few weeks you've been adding on to your todo app, rebuilding, and refactoring. For this Checkpoint you're going to rebuild this app into a Trello app that has three lanes: "Todo", "Doing", and "Done". Each app will have statuses that will help you filter the items into the correct lane and each lane will be made by the same component: `listOfTodoItems`. -->

## ProjectTitle Rubric
<!-- @TODO ATTENTION: DEVELOPER, Every Checkpoint needs a rubric. A checkpoint, after all, is a test of the skills they've learned or haven't. Be sure to specify the specifications of this project and assign them point values that equal 100 points.  -->

1. **20pts** - Spec1
1. **20pts** - Spec2
1. **20pts** - Spec3
1. **20pts** - Spec4
1. **20pts** - Spec5
1. **Bonus +20pts** - Spec6

### ProjectTitle Objective
<!-- @TODO ATTENTION: DEVELOPER, Just like the overview in the pre-homework and class lesson we want to give the students context for what they'll be practicing in this project. -->

### ProjectTitle Example
<!-- @TODO ATTENTION: DEVELOPER, A picture, mock-up, gif demo, or website the show what the students are working toward. The point is, you have experience in building apps like this and you know where they're headed. It would be more helpful if they, too, knew where they are headed. This will give the students something to reverse engineer or setup a goal post to reach. -->

<!-- EXAMPLE of ProjectTitle Example
 * [Trello](https://trello.com) -->

 * [EXAMPLETITLE](url)

******

### Follow-up Video - ProjectTitle

<!-- @TODO ATTENTION: DEVELOPER, This section is intended to get the students started more quickly, clarify confusion, and push them further.

1) It must be created by the ACA/Circle Education.
2) Don't give them answers but provide hints and any specific instruction that need to be followed. -->

<iframe width="560" height="315" src="https://www.youtube.com/embed/nbFmHD4T04k" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<!-- @TODO ^^^ THIS PLACEHOLDER VIDEO BELOW BETTER BE REPLACED!!!!! ^^^ -->

******
******

<!-- EXAMPLE RUBRIC:

1. **20pts** - Correct files:
    * `listOfTodoItems` - component that maps over the items give to it and renders a view of each item in:
    * `todoItem` - component that lists the details of the todo item and has buttons to:
        * "Mark as Done" -or-
        * "Mark as Doing"
        * "Delete"
        * "Update"
    * All actions that happen to a todo item will be in `todoServices`
    * Each item will implement a interface/model called `ITodo` which is shaped as follows:

        ```typescript
          export interface ITodo {
            id: number;
            title: string;
            isDone: boolean;
            isDoing: boolean;
            isEditing: boolean;
          }
        ```

1. **20pts** - Can update item
1. **20pts** - Can move item from one lane to the next
1. **20pts** - Can delete item
1. **20pts** - Utilizes a modal to confirm deletion of item
1. **Bonus +20pts** -
    * todo items change font color when moved to "Doing"
    * todo items are crossed out when moved to "Done" lane
  
-->

{% include "../includes/footer.md" %}