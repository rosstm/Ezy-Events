# Ezy-Events
## Step 1 Homepage code

Two raw content elements one with the embed code for the featured events and one for the repeating events, both set to tile. 
```
<div id="masonry_listing_featured" class="homepage_events"></div>
<script src="https://ezyevents.australianclubs.com.au/wp-content/plugins/EzyWebEvents/ezywebevents.js?updatecache" type="text/javascript"></script>

<script>EzyWebEvents(0000,'masonry_listing_featured', 'facebook','tile',2);</script>
```

```
<div id="masonry_listing_repeat" class="homepage_events"></div>
<script>EzyWebEvents(0000,'masonry_listing_repeat', 'ezyevents','tile',9);</script>
```

The ID (0000) needs to be updated.

## Step 2 Check What's On page code

As long as the embed code is set to Masonry, which most should be, you shouldn't need to change anything on the What's On page.

    <div id="masonry_listing"></div>
    <script src="https://ezyevents.australianclubs.com.au/wp-content/plugins/EzyWebEvents/ezywebevents.js?updatecache" type="text/javascript"></script>

    <script>
    EzyWebEvents(0000,'masonry_listing', 'both','masonry',16);</script>


## Step 3 CSS

1. Go to Cornerstone > Theme Options 
2. Click the CSS button and switch to the Global CSS tab.
3. Comment out the existing EzyEvents custom CSS. Each site should be similar but will have slight variations.
4. Add the [updated CSS from style.css](style.css)
5. The font type, size, colour and tile background colour will all need to be updated
