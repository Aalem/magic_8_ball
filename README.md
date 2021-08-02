# Magic 8 Ball (Challenge)

The final version of the application should look like this:  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/app_anim.gif" height="500">  

There are 6 ball images in the **images** folder of the project  

## Guide

### Step 1 - Create a Stateless Widget  
Create a new **Stateless** widget called **BallPage** in your main.dart file.  
Replace the word **null** with the new Stateless Widget you created.  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/1.png" height="250">  
  

Your **BallPage** should have a **Scaffold** with an **AppBar** and an empty **Container** as the body.  
The AppBar should have a blue **backgroundColor** and a **title** that says **'Magic 8 Ball'**.  
The background your Scaffold should have a white color.  
Once you run the app this is what you're aiming for:  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/2.png" height="500">  

### Step 2 - Create a Stateful Widget
Create a new **Stateful Widget** called **Ball** in your main.dart file.  
Instead of BallPage having a body of **Container()** replace it with your new Stateful Widget.  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/3.png" height="400">  

Your **Ball** Stateful Widget should display the **ball1.png** image. (You don't have to touch the pubscpec.yaml file)  
Make sure the image is **centred**.  
When you run the app this is what you're aiming for:  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/4.png" height="500">  

### Step 3 - Make it Interactive  
Use a **TextButton** Widget to make the Image clickable.  
Add a **print** statement that gets triggered when the button is pressed. It should print **'I got clicked'**.  
When you run the app and click on the ball image you should see the words "I got clicked" into the console like this:  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/5.png" height="250">  


### Step 4 - Randomise it
Inside the curly braces of **_BallState** create a **variable** called **ballNumber** that can only hold integers (**int**), set it to equal 0.  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/6.png" height="500">  

Instead of hard coding the ball image name that's being displayed on screen, use the **ballNumber** variable you just created instead.  
Add the **dart:math** library to your main.dart file.  
When the button gets pressed, use the ***Random()** generator and the **nextInt()** method from the dart:math library to generate a new ballNumber **between 0 - 5**.  
**print** the ballNumber to the console when the button gets pressed.  
When you **run** the app and **click** on the ball image you should see random number between **0 - 5** printed in the console like this:  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/7.png" height="250">  

### Step 5 - Update the State
Change the random numbers that are generated for **ballNumber** from 0 - 4 to 1 - 6 to match our ball image names.  
Instead of using a hard coded image name to display the ball image that's shown on screen, use **String interpolation** and the **ballNumber** variable instead to make it show a random image.  
Use **setState()** to update the state of the image when the **ballNumber** variable updates.  
All going well, you should now have the full functionality of the Magic 8 Ball app, it should look like this:  
<img src="https://github.com/Aalem/magic_8_ball/blob/master/git_images/app_anim.gif" height="500">  
