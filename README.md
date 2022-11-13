## Drink Water Reminder Project

The most effective way to keep ourselves healthy is to keep ourselves hydrated,and we often tend to forget to drink water so we are going to create a ‘Drink Water’ Reminder or Notifier app using Python which will remind us to drink water periodically.

### Modules Required
1. Plyer : Plyer is a platform independent module in python, that helps us to access  various features of our hardware / platforms like display notification , access sensor data ,play/pause audio etc

2. Time : There is a popular time module available in Python which provides many ways of representing time in code, such as objects, numbers, and strings.

### Installation:
* Time module comes with python, so we don’t need to install it. On other hand, plyer is not a build in module. We have to install it .
* Firstly, we have to open command prompt in administrator mode. Then, enter command

```
pip install plyer

```

### Approach:

Step 1: First we have to import the time module, and from plyer we will import notification.

```
from plyer import notification
import time 
```

Step 2: Second we have to call the notify method of the class. In this case, the parameters of the method is Title (title of our notification), Message (required message of our notification) and timeout (reqrequired time for displaying the message or notification , we have set it to 10).

```
notification.notify(
             title="......",
             message=".......",
             timeout=10
     ) 
```

Step 3: Finally,  we will add a sleep function to show the notification again after some time .

```
 time.sleep (60 * 60)
```

It means ,after every 60 minutes or one hour it will remind us or notify us to drink water.
