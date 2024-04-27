# Runner game inspired by Google Dinosaur and Pokemon

# Features Added:
1) Lives functionality - User has 3 lives when the game begins.
2) 1up and collision - User gains an additional life when the player collides with a heart icon in the game
3) Enahnced background, jump and collision audio

# Details
1)Lives functionality:
- Used Flaticon(https://www.flaticon.com/) to download pixelated icons and color them according to the game theme
- Created heart-class that is a sprite-group
- Animated the hearts by creating 2 different heart-designs and alternating between the 2 images to create an illusion of a video
- A new heart is created based on a random probability which has a 1-in-7 chance every second.
- If the user collides with a heart, then the user gains a new life
- If the user colllides with a snail or a bird then the user loses a life
- The game ends if there are no lives left or the user exits the pygame window

![](https://github.com/farhanahraf03/Pokemon-Runner/blob/master/gifs/Obstacle-Collision.gif)


2)1up and collision:
- 1ups are added in the form of hearts
- Collision are detected using pygame.spritecollide()
- There are 2 types of collisions:

    a) Collision with an obstacle:
    - Obstacles are birds or snails
    - Collision results in loss of a life
    - If the user collides with an obstacle, then all the obstacles and hearts in the current frame are also cleared so that user can have a fresh start

![](https://github.com/farhanahraf03/Pokemon-Runner/blob/master/gifs/Obstacle-Collision.gif)
       
    b) Collision with a heart:
    - Collision results in gaining of a life
    - If the user collides with a heart, then all the hearts in the current frame are also cleared so that the user cannot overload on extra lives

![](https://github.com/farhanahraf03/Pokemon-Runner/blob/master/gifs/Heart-Collision.gif)



