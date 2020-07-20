# Customizing Instructions: IDL-MD Syntax

!INSTRUCTIONS[Favorite Food Intro](https://raw.githubusercontent.com/LODSContent/lod-training/master/favorite-food/intro.md)

Login to the VM using the following information:

|Key|Value|
|--|--|
|Username|++@lab.VirtualMachine(LODTraining).Username++|
|Password|++@lab.VirtualMachine(LODTraining).Password++|

[Checkout Our Slack Community!](http://labauthor.slack.com/ "LODS Slack Community")

> [bash-code]:
> ```BASH-notab-nocopy-nocolor-linenums
> echo "My favorite 
>     food is:
>         @lab.Variable(food)"
> ```

In the box below, type the name of your favorite food:  
@lab.TextBox(food)

@lab.Activity(favfood)

All Foods are Good!<sup id="link1">[1](#ref1)</sup>

Select the food you would like to learn more about: @lab.DropDownList(option)[None,Salad,Chicken]

:::salad(option=Salad)

A salad is a mixture of small pieces of food.

:::

:::chicken(option=Chicken)

Chicken is the most common type of poultry in the world.

:::

!INSTRUCTIONS[Selected Food](https://raw.githubusercontent.com/LODSContent/lod-training/master/favorite-food/@lab.Variable(option).md)

===

# Customizing Instructions: Working with HTML

<font size=5 color=blue>&lt;<mark>This</mark> is a Placeholder&gt;</font>

`<This is a Placeholder You Should Copy>`

<details>
<summary>Food Examples</summary>

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

</details>

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

**References:**

<sup><strong id="ref1">1 </strong></sup>Not all people will think all foods are good. But different people think that different foods are good.[ ↩](#link1)
