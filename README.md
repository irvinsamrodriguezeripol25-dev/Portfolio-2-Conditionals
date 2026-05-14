# Portfolio-2-Conditionals

#Personal Mood Checker

### (I created this program ometimes do not notice how they feel throughout the day. 
### This program helps to quickly identify their mood and receive simple feedback or 
### encouragement based on their mood rating.)
### (I named this checker Mood Sense and has a AI assitant called Moodi.)

```python
print("=== Mood Sense ===")
print("Moodi:Hello I am Moodi, I'll be your Mood Sense Assitance for today! :3.")
print("Moodi:Kindly enter your name and mood for today, please :3.")
print("Moodi:On a scale of 1-10, how would you rate your day :3.")

name = input("Enter your name:")
mood = input("Rate your mood today (1-10): ")

try:
    mood = float(mood)  
```
### (I use float so that it still accepts decimal numbers.)

### (I made this part handle to the negative numbers, zero, and numbers above 10)

```python
    if mood <= 0 or mood > 10:
        print("Moodi: Please enter a number from 1 to 10 only :3.")
```
### (This range represents a sad or difficult mood.)

```python 
    elif mood >= 1 and mood <= 4:  
        print("Moodi:", name + ", Today seems a little difficult. :<")
        print("Moodi: Take some rest and do something you enjoy. :3")
```
### (Prints a message for users with a sad or difficult mood.)
    
### (This represents a neutral mood.)

```python
    elif mood == 5:
        print("Moodi:", name + ", You're in the middle today. :3")
        print("Moodi: Keep going, things can still get better. :3")
```
### (Prints a message for users with a nuetral mood.)
    
### (Represents a good or okay mood.)

```python
    elif mood >= 6 and mood <= 8:
        print("Moodi:", name + ", Your day seems okay. :D")
        print("Moodi: Keep that positive energy going.:D")
```
### (Prints a message for users with a good or okay mood.)

### (Represents a very happy mood.)

```python
    elif mood >= 9 and mood <= 10:
        print("Moodi:", name + ", You seem happy today! ^v^")
        print("Moodi: Looks like you're having an amazing day! :D")
        print("Moodi: Keep that positive energy going, " + name + ". :3")
        print("Moodi: Spread your good vibes to others. ^v^")
```
### (Prints a message for users with a very happy mood.)

```python
except:
    print("Moodi: Error: Please enter numbers only. :3")
```
### (Shows an error message telling the user to input numbers only.)
