# Ezy-Events
## Step 1 Homepage code

1. Go to Cornerstone > Page Builder > Home 
2. The homepage should have 2 seperate raw content elements one with the embed code for the featured events and one for the repeating events, both need to be set to tile and have the class "homepage_events". You can replace the existing embed codes with the 2 below, just make sure to update the EzyEvent ID.

![Screenshot of homepage](/screenshots/Screenshot%202022-05-27%20at%2015-59-11%20Home%20-%20Page%20Builder%20-%20Pro.png)

```
<div id="masonry_listing_featured" class="homepage_events"></div>
<script src="https://ezyevents.australianclubs.com.au/wp-content/plugins/EzyWebEvents/ezywebevents.js?updatecache" type="text/javascript"></script>

<script>EzyWebEvents(0000,'masonry_listing_featured', 'facebook','tile',2);</script>
```

```
<div id="masonry_listing_repeat" class="homepage_events"></div>
<script>EzyWebEvents(0000,'masonry_listing_repeat', 'ezyevents','tile',9);</script>
```

3. The ID (0000) in this code needs to be updated to the websites EzyEvent ID.
4. Click Save to commit the changes.

## Step 2 Check What's On page code

As long as the embed code is set to Masonry, which most should be, so you shouldn't need to change anything on the What's On page.

    <div id="masonry_listing"></div>
    <script src="https://ezyevents.australianclubs.com.au/wp-content/plugins/EzyWebEvents/ezywebevents.js?updatecache" type="text/javascript"></script>

    <script>EzyWebEvents(0000,'masonry_listing', 'both','masonry',16);</script>


## Step 3 CSS

1. Go to Cornerstone > Theme Options 
2. Click the CSS button and switch to the Global CSS tab.
3. Comment out the existing EzyEvents custom CSS. Each site should be similar but will have slight variations. 
4. Be careful not to remove or comment out other custom CSS not related to EzyEvents as that could break other features on the website.

![Screenshot of homepage](/screenshots/Screenshot%202022-05-27%20at%2016-05-39%20Theme%20Options%20-%20Pro.png)

5. Add the [updated CSS from style.css](style.css)
6. The font type, size, colour and tile background colour will all need to be changed to match the site style. You should be able to copy and paste these attributes from the commented out CSS. 
7. All changes will be shown live, so you can adjust font-size etc and see the changes before committing them.
8. Once the fonts and colours look right, click Save.
9. The Home page and What's On pages should now be updated with the new layout.
