We extracted all of the elements from the poster and placed the SVG code directly into the index.html file. After reading the descpription of the oblig we thought this was the way we were supposed to do it.

The SVG code came with styling, so we had to remove that from the index.html and add it to the styles.scss. We changed the class names for the SVG's and the paths so that it became more understandable which element it belonged to and what it did.

Then we placed the SVG elements using top and left so that it would look like the original poster.

Then we decided which elements we would animate and how we would achieve the result we wanted. We decided to animate the two stars beside the moon, the car and some of the clouds.

After we were done and felt ready to deliver, we discovered that there were several issues with browser compatibility regarding the animations. All the animations work on Firefox, but on Chromium-based browsers the car SMIL path animation for the car doesn't work, while on Safari none of the SMIL animations seem to work. We don't know how to make the animations work for all browsers, and we don't have the time to look into it since we discovered this problem very late.

Animated some of the clouds using animateTransform type="translate" to make it move side to side to make a "shiver" effect.
Some of the other clouds is animated using animateTransform type="scale" to make them scale up and down in size.
By adding animations to the clouds we felt that it highlighted one of the keypoints that the poster is trying to emphasize, that each and every one of us must try to minimize our carbon footprint.
https://developer.mozilla.org/en-US/docs/Web/SVG/SVG_animation_with_SMIL

The stars next to the moon were animated using CSS keyframe rotate animations. Very simple animations that fit the objects without needing much code. Meant to make the stars look like they're twinkling/sparkling in the sky. [Code from geeksforgeeks](https://www.geeksforgeeks.org/how-to-shake-an-image-using-css-keyframe/)

The car got a curved SMIL path animation, in order to highlight the point made about TikTok and trips to the moon.
[Code from Mozilla Developer.](https://developer.mozilla.org/en-US/docs/Web/SVG/SVG_animation_with_SMIL) Unlike the other elements that used position absolute, the car was not responsive for smaller screens, despite being positoned like other elements using percentage values. An attempt to fix this was made using several media queries, but it still doesn't look quite right on smaller screens.

The pupils of Earth's eyes were added by using CSS drawing, and then a keyframe animation was added to make the eyes shake. This is to show that the Earth is worried about all the pollution going on.
