# Customizing Instructions: IDL-MD Syntax

!INSTRUCTIONS[Favorite Food Intro](https://raw.githubusercontent.com/LODSContent/lod-training/master/favorite-food/intro.md)

Login to the VM using the following information:

|||
|--|--|
|Username||
|Password||

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

Select the food you would like to learn more about: @lab.DropDownList(option)[None,Salad,Chicken]

:::salad(option=Salad)

A salad is a mixture of small pieces of food.

:::

:::chicken(option=Chicken)

Chicken is the most common type of poultry in the world.

:::

!INSTRUCTIONS[Selected Food](https://raw.githubusercontent.com/LODSContent/lod-training/master/favorite-food/@lab.Variable(option).md)
