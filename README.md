# Deep Learning for Automated Discourse
# Assignment 1: Alexa Skill

## Description
We created a "Mimic Skill" with multiple custom intents:

1. A ``mimic`` intent where Alexa repeats what the user said back to the user if they prefix their statement with "mimic"
2. A ``hello`` intent where Alexa says "Hello" back to the user
3. A cute joke ``stop`` intent that the user invokes with "stop copying me"

And for fun we made it sassy.

## Example Discourse
The user is prefixed with ``>>`` and Alexa's resonse is below.
```
>> Open mimic skill
Welcome to Mimic, where I repeat back to you exactly what you said, so you know how stupid you sound. I also say hello.
>> mimic I'm Aaron
you said I'm Aaron
>> hello
Hello, there!
>> mimic actually, I'm Alexandra
you said actually, I'm Alexandra
>> stop copying me
you said, stop copying me. Just kidding, goodbye.
```
