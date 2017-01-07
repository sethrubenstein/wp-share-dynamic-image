# wp-share-dynamic-cards
Lets you share a post while changing the image, title, description for the shared card.

The url structure is `{site_url}/share/{post_id}/{image_id}` where {site_url} is obviously your site's url and {post_id} is the post whose permalink, title, excerpt you wish to share while {image_id} is the image you want to use in your media library.

## Filters
`wpsdc_site_name` lets you change the site name used in Facebook OG:site_name - otherwise defaults to `bloginfo('name')`.

`wpsdc_twitter_username` lets you pass the site's Twitter username.

`wpsdc_twitter_creator` lets you pass a specific user's twitter username associated with this image/article. It's up to you to develop this out.

`wpsdc_image_size` in the even that you have a custom image_size that you define for shareables - othwerise defaults to large.

## Helper Functions
`wpsdc_get_share_url($postID, $imageID)` will return a url with the correct url structure. All you need to do is pass the postID you want and the imageID of the image you want to retrieve from the ML.