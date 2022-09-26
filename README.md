# Car_Distance_Project
This project allows you to use object detection to tell the color, model, and distance between certain cars.

# Learning Outcomes 💫

By the end of this blog post, you will be able to…

- Know what features make a rectangle or polygon for computer vision applications
- Understand how to calculate distance between two points / objects in an image or video
- Convert pixel distance to real world measurements
- Conceptualize how estimating distance can be applied to other use cases

# Calculating Distance Between Points for Computer Vision

To calculate distance between two points we can use the Pythagorean Theorem to solve for any side of the polygon.

![image](https://user-images.githubusercontent.com/113200203/192389070-d8302ee0-dfe9-481e-8c5a-61f04dc45a7c.png)

Often in computer vision problems you are solving for side c, because you are trying to calculate the distance between two object points that are on different horizontal and vertical planes.  

By using the coordinates (x1, y1) representing the right most point on the triangle and coordinates (x2, y2) representing the top most point.

We can use a^2 + b^2 = c^2 to determine the distance between two points.

> **Lines 114 - 215 in Car_Detection_and_Color.py** 
