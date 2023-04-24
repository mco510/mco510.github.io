
## Using github online

This is the new front page for the MCO510 pages. 

You can create links to other documents -- it's easiest to do this yourself. 

Say you create a Quarto document, which in turn creates an HTML. As long as you have used the option `embed-resources: true`, all you need to do is to upload that document. 

Here's an example, with my first markdown document with a moose: [first-markdown.html](first-markdown.html)

Here are some basic instructions: 

1. Create an account at github.com 
3. Create a new repository. 

You have to make some decisions now. Do you want this to be a "home" page, or do you want it to be a "project" page? I suggest "project", but something with your name in it. This makes it easier for you to decide to change it later. 

Once you have done that, 

1. Go to "Pages". I suggest changing the default "<root>" directory into "docs". That means that any html page that you copy should go into your docs folder. You don't have to do this. 
  
2. Go to the [Github supported themes](https://pages.github.com/themes/) page and choose one. This is a slightly different set of templates that you saw in R. The list of supported themes is [here](https://pages.github.com/themes/). They aren't quite as nice. 
  
3. When you get there, look for the `_config.yml` page, and copy the text. Create a `_config.yml` file in your "docs" folder, and paste it in. 
  
## Using github from the app
  
You can also download the app, and use github that way, by transfering your site back and forth. However, it's a little hard to do that with this basic setup without also loading the program that converts this markdown into a site. 
  
## Using github from R
  
Another way to do this is to set up your site as a project in R. Then put your programs, etc, in the root directory, and tell it that you want to use it in docs. I'll show you this in class. In this case, we skip jekyll completely, and then just use the RStudio program to manage our conversion and commits. 
  
  
  
 There are a few technicalities you have to get through before you can publish through RStudio. 
  
  * Set up a "personal access token", or PAT. You will use this instead of your password when you set up your site to publish. Here are some step-by-step directions for this: <https://gist.github.com/z3tt/3dab3535007acf108391649766409421>
  
  * Change the publish directory in both your project YAML and your github site to "docs" 
  
  * Add a file calle .nojekyl to the root directory. This prevents the default github behavior of turning markdown into HML. 
  
  
  
