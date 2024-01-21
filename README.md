# ReadingAid
A simple app for helping people read, through live feedback and visual aids. This uses ChatGPT 4.0, AssemblyAI.

## How to use
The app is configured to run with Flask. If you have Python and Flask, you can clone this repository, write `pip install -r requirements.txt` and run it using `flask run`.

The app takes user input and gives a sample to read using OpenAI's Chat SDK. The system is configured using the following query:

`Students will provide you with short reflections on emerging trends in the business world. Evaluate the reflections in terms of spelling and grammar, and in terms of evidence of critical thought. Provide a grade between 0 and 10, where 0 represents a very poor response and 10 represents a fantastic response.`

The site then writes ChatGPT's response in the space below the button.

## Sample paragraphs
Need some sample paragraphs to read? Consider copying and pasting the following to see ChatGPT's assessement.

### Expert
> Thomson Reuters has a wide range of digital transformation products and is well-positioned to lead in this space. The  company has some of the leading real-time news sources, which has allowed them to develop advanced natural language processing tools, which they have tailored to professional services automation. They are likely to leverage this advantage, as there are few companies that have both the resources and capabilities to develop novel generative AI, due to the complexity of procuring and retaining vast quantities of novel data.

> I appreciated Walmart's implementation of sustainable practices. Their implementation of LED lighting and sustainable energy will likely have a measurable impact. I am not sure whether this is an example of greenwashing, though, because they provided their statistics in cumulative terms, rather than their annual emissions reductions.

### Intermediate
> I think Thomson Reuters provides news. I don't really see how this makes them a technology leader.

> Walmart suuuuucks and its shares are gonna tank. Nobdy buys stuff from them.

### Beginner
> I think Thomson Reuters provides news. I don't really see how this makes them a technology leader.

> Walmart suuuuucks and its shares are gonna tank. Nobdy buys stuff from them.

A huge shout out to the OpenAI Quickstart repository at https://github.com/openai/openai-quickstart-python
