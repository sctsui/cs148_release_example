# cs148_release_example


# To create a tag:
## Option 1: Web UI
* You can use the web UI to create a tag, but it will only create the tag from the current version (most recent commit).
The tag is automatically created when you create a new release in the git UI.
* Skip directly to 'Create a Release'

## Option 2: command line instructions. 
(Choose this option if you need to create a tag that is earlier than the most recent commit)

`git tag v1.0.0 <commit ID>`

note - v1.0.0 is the tag name, and commitID refers to the last commit in your MVP 

you can find the commit ID using `git log`, or using the history tab in the github web ui

if done correctly, you should see something like this in the git log
![image](https://user-images.githubusercontent.com/10558897/116512519-06006680-a87d-11eb-9ead-d6cbc0d633bd.png)

if you messed up, you can delete the tag using `git tag -d <tag_name>`

Verify that everything looks good, then `git push origin <tag_name>`

Your newly created tag should appear in your tags page on the web UI

# To create a release:

## Option 1:
* If you want to create a release from the current, most recent commit
* On the right hand column, there should be a section labeled 'Releases'. Click on 'create a new release'
* Put v1.0.0 in the 'Tag Version' box, and fill out the rest of the boxes.
* Click `Publish Release' and the tag will automatically be created for you

## Option 2:
* If you want to create a release from an existing tag
* On the right hand column, there should be a section labeled 'Releases'. Click on 'create a new release'
* There should be a toggle between Releases and Tabs right above the 'Tag Version' form. Click on Tabs to toggle over.
* Click on the  menu (with 3 dots) on the far right hand side of the tag, and select 'Create Release'
* Fill out the form, and `Publish Release`
