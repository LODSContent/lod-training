# IDLx Markdown Syntaxes

## Markdown Explanation and Editor Navigation
1. Explain Markdown (Generally)
    1. PowerPoint

1. Explain IDL-Md (Specifically)
    1. PowerPoint

1. Preview "WYSIWYG" Editor

    1. On line 1 of the instruction editor, type `Customizing Instructions:`

    1. With no whitespace at the end of your line, move to line 2.
    
    1. On line 2 of the instruction editor, type `IDL-MD Syntax`

    1. On line 1, add 2 spaces at the end.

    1. On line 1, remove the added spaces and press **Enter** to create a new empty line below it.

    1. Combine all text to sit on line 1

1. Brief Walkthrough of Cheat Sheet and "Learn More"

    1. Make Line 1 a level 1 header.

    1. Move Cursor to line 3.

        1. Discuss Best Practice - Empty line between components, even if they put one on their own.

## Replacement Tokens

1. What are replacement tokens?
    1. PowerPoint?

1. When to use replacement tokens
    1. PowerPoint?

1. How to find valid replacement tokens

    1. On line 3, add the following:
    
        ```
        Login to the VM using the following information:

        |Key|Value|
        |--|--|
        |Username||
        |Password||
        ```

    1. On line 7, in the second column (after Username) use the @lab Listing to add the VM Username Replacement Token

    1. On line 8, in the second column (after Password) use Intellisense to add the VM Password Replacement Token. 
    
## Link Descriptions

1. Why are they important?

1. On line 10, add the following URL `[Checkout Our Slack Community!](http://labauthor.slack.com/)`

1. Hover over the link in the preview and note that nothing obvious happens.

1. At the end of the URL (within the parentheses), add a space and the following text `"LODS Slack Community"`


## Code Blocks + Modifiers (Optional)

1. What are Code Blocks?
    1. PowerPoint?

1. On lines 12+13, add the following

    ```
    ```
    ```

1. Add the following text between lines 5+6 with the following text 
    
    ```
    echo "My favorite 
        food is:
            Grapes"
    ```

1. On line 12, add `BASH` to the end of the backticks

1. On line 12, after **BASH** add `-notab`

1. On line 12, after **-notab** add `-nocopy-nocolor-linenums`

## References/Includes

1. What are they and why use them?

### References

1. Add an empty line below line 11, moving the code block that begins on line 12 down.

1. On line 12, add the text `> [bash-code]:`

1. Using the Ctrl+Alt+Shift keyboard command, select lines 13-17 and add a > and a space to the beginning.

1. Preview the command palette where more keyboard shortcuts can be used.

1. On line 19, add the text `!INSTRUCTIONS[Click to View Code][bash-code]`

1. On line 19, change the !INSTRUCTIONS to a `^`

### Includes

1. On line 3, add the text `!INSTRUCTIONS[Favorite Food Intro](https://raw.githubusercontent.com/LODSContent/lod-training/master/favorite-food/intro.md)`

1. Remove Lines 21 and 22.

## Textbox/Variables

1. On line 21, add the following text:

    ```
    In the box below, type the name of your favorite food:  
    @lab.TextBox(food)
    ```

1. On line 24, type ++@lab\.Variable(food)++

1. In the preview pane, type your favorite food.

1. Remove line 24.

1. Press Ctrl+H to open Find+Replace.

1. Search for **Grapes** and replace with ++@lab\.Variable(food)++
    
    1. Optionally highlight Search options and use case sensitivity.

1. Show on line 18 where **Grapes** has changed.

1. Show in the preview where **Grapes** has changed.

1. Change your favorite food in the preview.

1. Show that the code block updates.

## Activities

1. Open Lab and Refresh Screen

1. Open the instruction editor and ensure your cursor is on line 24.

1. Open the activities editor and create an unscored automated activity.

1. Configure the following fields:

    |||
    |--|--|
    |Name|++Post Favorite Food++|
    |Replacement Token|++favfood++|
    |Custom Eval Button Text|++Create File++|

1. Paste the code block from the lab manual into the script field.

1. On the last line of the script field, add `$true`

1. Click **Save and Insert**

1. Review where to retrieve the token from in the future.

1. From the lab run the activity and verify the file is created on the desktop.

## Dropdowns/Divs

1. On line 26, add the text `Select the food you would like to learn more about: @lab.DropDownList(option)[None,Salad,Chicken]`

1. On line 28, add the text below:

    ```
    :::salad
    :::

    :::chicken
    :::
    ```

1. In the new **Salad** section, add the text ++A salad is a mixture of small pieces of food.++

1. In the new **Chicken** section, add the text ++Chicken is the most common type of poultry in the world.+++

1. Show that both items appear in our preview pane, and that changing the dropdown does nothing.

1. On line 28, add the following text after the word salad (with no space in between) ++(option=Salad)++

1. On line 34, add the following text after the word salad (with no space in between) ++(option=Chicken)++

1. On line 40, add the text `!INSTRUCTIONS[Selected Food](https://raw.githubusercontent.com/LODSContent/lod-training/master/favorite-food/None.md)`

1. In both the image and the include, replace **None** with ++@lab\.Variable(option)++

1. Verify Everyone has 40 lines of code.

===

# Adding HTML Components

1. On line 42, add the following text to make a new page ++===++

1. On line 44, add the following text ++# Customizing Instructions: Working with HTML++

## HTML "Tag" Escaping

1. On line 46, add the following text `<This is a Placeholder>`

1. On line 46, replace **<** with `&lt;` and replace **>** with `&gt;`

1. On line 48, add the following text `<This is a Placeholder You Should Copy>`

1. On line 48, add a backtick (`) to the beginning and end of the line.

## Basic HTML Tags

1. On line 46, add `<font size=5 color=blue>` to the beginning and `</font>`

1. Switch between light and dark theme to notice the impact

1. On line 46, replace **This** with `<mark>This</mark>`

1. Switch between light and dark theme to notice the impact

## HTML Divs

1. On line 46, add a `<div>` and move the existing content down.

1. On line 52, add a `</div>`

1. Review the disappearing content in the preview.

1. Remove the div openings and closings

## Details/Summary Sections

1. On line 50, add the following text:

    ```
    <details>
    <summary>Food Examples</summary>
    </details>
    ```

1. Create a new line between line 51 and 52 with the following text, ++Apples are fruit and Brocolli is a vegetable++

1. Replace line 52 with the following text (include an empty line before and after the section):

    ```
    <details>
    <summary>Fruits</summary>
    - Apples
    - Bananas
    </details>

    <details>
    <summary>Vegetables</summary>
    - Brocolli
    - Carrots
    </details>
    ```

## Tables

1. On Line 67, add the following text

    ```
    <table>
        <tr>
            <th colspan="2">Fruits</th>
            <th>Vegetables</th>
        </tr>
        <tr>
            <td>Gala Apples</td>
            <td>Granny Smith Apples</td>
            <td rowspan="2">Brocolli</td>
        </tr>
        <tr>
            <td>Bananas</td>
            <td></td>
            <td></td>        
        </tr>
        <tr>
            <td></td>
            <td></td>        
            <td>Carrots</td>
        </tr>
    </table>
    ```

## References

1. On line 26, add the following text `All Foods are Good!<sup id="link1">[1](#ref1)</sup>`

    1. Move the existing lines down to make room.

1. On line 91, add the following text:

    ```
    **References:**

    <sup><strong id="ref1">1 </strong></sup>Not all people will think all foods are good. But different people think that different foods are good.[ ↩](#link1)
    ```
