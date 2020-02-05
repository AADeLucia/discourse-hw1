# Deep Learning for Automated Discourse
## Assignment 1: Alexa Skill
## Alexandra DeLucia, Aaron Mueller

### Description
We created a "Mimic Skill" with multiple custom intents:

1. A ``mimic`` intent where Alexa repeats what the user said back to the user if they prefix their statement with "mimic."
2. A ``hello`` intent where Alexa says "Hello" back to the user.
3. A cute joke ``stop`` intent that the user invokes with "stop copying me."

And for fun, we made it sassy.

### Reproduction Steps
To reproduce our skill's functionality, follow these steps:

1. Log in to your Alexa Developer Console.
2. Go to the "Build" tab. Under "Interaction Model", click "JSON Editor."
3. Copy the contents of `interaction_model.json` into the JSON editor box, replacing the existing content.
	- Save the model, then build it by using the appropriate buttons above the editor.
4. Go to the "Code" tab. Replace the contents of `lambda_function.py` in your interface with the contents of our `lambda_function.py` file.
	- Save and then deploy the code using the appropriate buttons above the code editor.
5. Now, go to The "Test" tab or `Echosim.io`
6. Say "open mimic skill". Now, you should be able to use all of our custom intents!
	- This skill will not automatically close after performing one action. However, it can time out if you do not say anything for a few seconds. If this happens, try reopening the skill.
	- To use our `HelloIntent`, say "hi" or "hello" to Alexa.
	- To use our `MimicIntent`, say "mimic" and then a phrase you want Alexa to repeat.
	- To close the skill with style, say "stop copying me." Alexa will have a cheeky response.

### Example Discourse
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
