# Dev Test

## Instructions

The goal of this test is to create a [Craft 3](https://docs.craftcms.com/v3/installation.html) application. The application should:

- Allow a user to open the homepage in a browser
- Return 20 restaurants from Melbourne CBD in the homepage using in the homepage using the [Yelp search endpoint](https://www.yelp.com/developers/documentation/v3/get_started) in a JSON format using twig
- Import the restaurants in the CMS

You will be evaluated on:

- Showcasing your ability to create PHP code to contact the Yelp API
- Showcasing usage of PHP standards / best practises
- Showcasing relevant and up-to-date technologies to install and render the app on a computer
- Showcasing usage of Craft 3
- Showcasing usage of Git
- Showcasing any relevant Backend tech
- Showcasing ability to write documentation to install/run/test this project

Do as much as you can and provide a Github repository link with relevant commits (including any dev tools you used). Please include any relevant instructions for someone else to install your app.
Don't install third party plugins, write your own to integrate with the Yelp API and import restaurants in the Craft CMS

## Documentations

To help you start quickly with Craft without spending too much time on setting it up, we have included some details on how this might work.

There are several ways you might want to tackle the Yelp implementation in Craft but one way might be by using a Twig function in your homepage template. Please find documentations below to help you achieve that quickly but it doesn't mean you have to go down that road.

- [Yelp](https://www.yelp.com/developers/documentation/v3/get_started)
- [How to build a Homepage](https://docs.craftcms.com/v3/sections-and-entries.html#singles)
- [How to Build a Module](https://docs.craftcms.com/v3/extend/module-guide.html)
- [Register a Twig Extension](https://docs.craftcms.com/v3/extend/extending-twig.html#register-a-twig-extension)

You should also consider the following:

- What would happen if the Yelp API was down? Can you still load restaurants on the homepage?
- What about performance, is it the fastest approach? Do you need to load the API to display restaurants?
- What if you want to enrich the Yelp data in the CMS?

Bonus:

Import Yelp's category in the CMS. Your homepage will then only display restaurants belonging to categories that are enabled in the CMS. Finally importing restaurants from Melbourne CBD should only be based on enabled categories.