# Project Outline

### Overview 
The project is called Recipe Quest. It will allow anyone to search, by a category, i.e., Beef, Chicken, Dessert, or by area(country of origin) for recipes on a public API. The user must register/sign-in in order to view, add or delete a recipe to or from their "favorites" located in a MySql database.

As the person responsible for "What's for dinner?", I get tired of cooking and eating the same things all the time.
While there are probably hundreds of recipe websites out there containing thousands of recipes, it can sometimes take hours trying to pick one.  This public API contains unique recipes from around the world. This is the place to find something different.
### Features
Release 1:
a) Call an API to display a list of categories that can be selected for the recipe search. 
b) Call an API to display a list of areas(Italian, Chinese, Mexican) that can be selected for the recipe search.
b) Call an API by the selected category to gather all recipes for that category. Or Call an API by the selected area to gather all of those recipes.
c) Display all the recipes for the selected category or area by picture and recipe name. A recipe is selected by clicking on the picture.
d) The entire recipe is displayed for a selected recipe and the user can decide to save it to their "favorites".
e) Require the user to register/sign-in in order to access their "favorites" to view, add, or delete recipes. 

Release 2:
- I would like to include a search by main ingredient and the first letter of the recipe name. For example, gather all recipes that start with the letter "M".
- Include the functionality that allows a user to enter their own recipes and save them to their "favorites". Uploading a picture would be optional.  


### Technologies
a) ASP.NET MVC
b) C#
c) Bootstrap
d) MySql
e) Microsoft.AspNetCore.Identity.EntityFrameworkCore
f) Pomelo.EntityFrameworkCore.MySql
g) Microsoft.AspNet.WebApi.Client
h) *APIs for Release 1:
    - Contains a list of all meal categories: https://www.themealdb.com/api/json/v1/1/categories.php
    - Contains a list of all meal areas: https://www.themealdb.com/api/json/v1/1/list.php?a=list
    - Contains a list of all meals for a specific category(Seafood): https://www.themealdb.com/api/json/v1/1/filter.php?c=Seafood
    - Contains a list of all meals for a specific area(Mexican): https://www.themealdb.com/api/json/v1/1/filter.php?a=Mexican 
    - Contains the entire recipe for one specific meal by mealId: https://www.themealdb.com/api/json/v1/1/lookup.php?i=52772 
i) *APIs for Release 2:
    - A list of all meals that contain the searched main ingredient: https://www.themealdb.com/api/json/v1/1/filter.php?i=chicken_breast
    - A list of all meals that start with a selected letter: https://www.themealdb.com/api/json/v1/1/search.php?f=a

    * - More information about the APIs can be found at: https://www.themealdb.com/     

### What I'll Have to Learn
a) How to use Bootstrap to format my pages.
b) I will have to figure out how to deserialize the APIs, because they are in a different format than the ones I have used in the past.
Here's an example:
    {"meals":[{"strArea":"American"},{"strArea":"British"},{"strArea":"Canadian"}]}


   

     


### Project Tracker
https://trello.com/b/aI0WEcqR

