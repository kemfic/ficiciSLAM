# ficiciSLAM

A crappy visual SLAM implementation I'm working on to learn stuff


    - (WIP) only visual odometry works, currently
<p float="left">
  <img src="resources/scene.png" height="250" />
  <img src="resources/vo.png" height="250" />
</p>

## todo
   - redo frame updater
   - take a good hard look at how I'm triangulating points
   - add lucas kanade tracking, and option to use either ORB matching or LK
      - use the cool masking trick from the NASA presentation
   - optimizer!

## how to use
   - not sure if I can share the datasets i'm using, so just put any video file in the `vids/` folder

   - currently only have visual odometry barely working, so just run `python stream.py` to see it working

want to learn more about slam/visual odometry?
---
   - check out Multiple View Geometry by Hartley & Zissermann
   - [Avi Singh's visual odometry projects](https://github.com/avisingh599/mono-vo)
   - [twitchslam by geohot](https://github.com/geohot/twitchslam)
   - [UZH and ETH Zurich's course (Vision Algorithms for Mobile Robotics)](https://web.archive.org/web/20171231011504/http://rpg.ifi.uzh.ch/teaching.html)
   - PTAM, ORB-SLAM, LSD-SLAM
     - papers and code are super useful
   - OpenCV references in API documentation
     - look in the SFM modules

## Dependencies
   - OpenCV
   - Numpy
   - Scikit-image
   - pangolin (we use uoip's fork for its bindings, since its a bit more python-friendly and intuitive)
      - https://github.com/uoip/pangolin

## LICENSE

MIT license. Do what you want with it, but please attribute my work if you do. Also don't sue me.
