Angular Routing with UI-Router
==============================

Routing in the front-end can be just as important as routing on the back-end. UI-Router is one of the most popular routers for angular and is a staple for every angular application.

You are going to be dropped into an application that already has a few things set up for you. 

You currently have a `MusicService` that is populated with data but.... the service does not know how to return anything to any of the controllers.

####Step 1 Get the Service and Controllers Talking

 The `albumsComponent` and view have already been set up and are completely functional as long as your service and routes are working correctly.

 Start with the `MusicService` and then follow the comments from there.


###Step 2 Album Component

 The end goal for this application is to have it function similarly to Amazon or Itunes. Typically you will see a url look something like this.

 ```javascript
 var url = {
   protocol: 'https://',
   domain: 'www.amazon.com',
   resource: 'product',
   itemId: 'B00ZMVGTA2'
   full:"https://www.amazon.com/gp/product/B00ZMVGTA2"
   }                         // ^^ Not sure what that is there for ???
 ```

> One of the main reasons for building a url like this is so we can share links that will can dictate the exact state of an application.

Your goal is to build out this music app so you can share a link and send someone directly to your favorite album

your urls will end up looking something like this

http://localhost:8080/#/albums/557119 

To pull this off your `AlbumController` will need access to your AlbumService and call the method `getAlbumById` and pass in the appropriate property from your `$stateParams`.  As long as you built out your service and routes you should be able to attach that album to your `AlbumController` and start building your view for an individual album.   



## Legal Overview

The content under the CodeWorks®, LLC Organization and all of the individual repos are soley intended for use by CodeWorks Instruction to deliver Educational content to CodeWorks Students.

---

## Copyright

© CodeWorks® LLC, 2021. Unauthorized use and/or duplication of this material without express and written permission from CodeWorks, LLC is strictly prohibited.


<img src="https://bcw.blob.core.windows.net/public/img/7815839041305055" width="125">

