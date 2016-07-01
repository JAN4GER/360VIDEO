# 360VIDEO
360 video player with direction and elevation scripting

In  most cases, viewers of 360 video make some camera rotations at the begining of the video. Look left, right, top, down.
And (in most cases) they left the camera in less or more random direction for the rest of the video.
This can make invisible best parts of 360 view for users, becasue they do not know where it is (which direction).
Creators of 360 movies should have possibility to define timeline of camera direction and elevation.
When users do not manipulate 360 view, the view should change automatically. By its creator definitions.

1. I create HTML5 video player for 360 videos.
2. I use free three.js library to render 360 (panoramic) viewer.  https://github.com/mrdoob/three.js 
This is only one of possible solutions in three.js at this moment I do not care which solution is the best.
3. I use Javascript to read external txt file where I define timeline to control point of view. 
This is done line by line in format: video running time in seconds [space] direction 0-360 [space] elevation +/-90

Changing both direction and elevation should do smoothly by path calculated from current point of view.

When user make manipulation of point of view (camera), the defined timeline is paused.
When user stop/pause manipulation, the timeline back to work with camera rotation to the next defined direction and elevation in timeline (point of view).

In this case we can share 360 videos which will show users the most important parts of view, right defined by creators or publisher.

Case: is this make playing speed limited? Rotation smooth limted? Both on laptop and mobile devices?
