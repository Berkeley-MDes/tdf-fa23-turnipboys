# Report #9 Week of 10/24/2023

## Aylish Turner

### Reflections

After closing out project 2 with our ghost robot and ghost hunter device (digital ecosystems), I was very intrigued to learn about this new project! We only have a week to create a "digital me," or an AI assistant version of myself utilizing ZeroWidth and LLMs. I've trained neural networks for object recognition before, but I've never done anything quite like this.

I admit that I had some weird personal and ethical hesitations when it came to the concept of a "mini me," especially because we are also utilizing ChatGPT and online knowledge to feed in the bot's capabilities. Thus, it doesn't really represent ME at all. I feel a little bit weird about letting it represent me as a digital twin and am more interested in it being a type of "fraternal twin" rather than identical. I'm okay with it talking similarly to the way I do, but I don't think that it can ever truly represent me or my thoughts, no matter how much knowledge I give it.

#### Initial Experimentation

The founder of ZeroWidth, Peter Binggeser, gave us a really great tutorial and overview of LLMs as well as how our prototyping process will work. The following are my notes that I took in class about large language models and ZeroWidth:

- large language models (LLMs)
- steps to creating a LLM
    - pass a massive amount of raw text through a giant neural network
        - the model “learns” how to predict what word (token) comes next given a prior sequence of words (tokens)
        - results in a “pretrained model”
        - all it knows is how to complete the next token, not trained to hold a conversation
    - train on structured supervised prompt & response example data
        - model “learns” how to structure a specific response, carry a conversation, or specific desired task
        - fine-tuning
            - alters the raw parameters & weights
        - results in a fine-tuned model
        - importance of understanding fine-tuning
            - lean into phrases like “you” are an AI, “user” will give you a task
    - generate options & select the best one to reinforce the model
        - humans or more powerful models are used to judge the model’s response to specific prompts
        - results in a foundational model
            - AI systems w/ broad capabilities that can be adapted to a range of different, more specific purposes
- tokens
    - unit or chunk of text divided for analysis
    - 1 token ~= ~4 characters of text for common English text

I set up the initial Intelligence and decided to name it "Babylish" (baby me). I followed Peter's instructions in the demo by also created a new Babylish knowledge set. I had to manually add my information by copying/pasting my weekly reports in my Github. This is a good tutorial overview of ZeroWidth from Peter: https://www.youtube.com/watch?v=uC1_HnSn0vc

I know that the AI is meant to just kind of know things about my class projects, but I was curious to know if I could customize it a little more and let it know more about my personality through things like film, TV shows, games, etc. I downloaded my data from Letterboxd, a website where I log what movies I watched and what my thoughts are on them. I tried to upload the CSV files with my Letterboxd data, but ZeroWidth wouldn't accept the data. I then tried to convert the CSV data into markdown format, but it still didn't work. It seems like I have to type out the information in order for ZeroWidth to accept it. I messaged Peter to see if there was another way to upload CSV data and will update if I hear back from him.

In the meantime, I decided to play around with the AI and see what it knew. I gave it some basic instructions telling it that it was a digital assistant representing my projects, opinions, and thoughts. Curiously, when I asked the AI who it was, it assumed that I used she/her pronouns. My name is feminine, so this makes sense. I told the AI that I use they/them pronouns and it correct itself within the same conversation, but because the AI does not remember information across conversations it kept on using the incorrect pronouns in future conversations. I fixed this by manually telling it my pronouns in the instructions. This didn't bother me, but I found it very interesting that it assumed I was a female (I guess from my female name), since I feel like AI usually assumes that I am male.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-23%20180147.png)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-23%20180657.png)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-23%20180756.png)

I then wanted to see if I could get the AI to speak similarly to how I do. This was an interesting challenge because I have very different speech patterns depending on who I'm talking to. I'm much more formal in these reports, essays, and other online content, but in actual direct messaging and chats I'm very casual and tend to have worse punctuation and grammar.

I requested my data from Discord to see if I could acquire all of my chats and upload them to the knowledge set, but Discord said that it could take up to a month to receive my data back and I only had a week to create the AI. I decided to expedite the process a little bit by uploading a bunch of essays and texts I had written to the knowledge set.

Weirdly, after I uploaded information about my favorite movies, the AI pretty much only wanted to talk about movies. It said that it didn't have any information on my latest projects despite also having knowledge from my weekly reports.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-24%20151324.png)

I saved my LinkedIn information to a PDF and uploaded it to ZeroWidth, but it did not do a good job parsing through the information. I had to manually fix a lot of the formatting.

#### Further Customization

I thought that it would be more interesting to change the speech pattern of my assistant bot, so I wrote out a new set of Instructions telling the AI to type in a similar way as I would. I told it a few key phrases/words that I always say as well as the emoticons that I frequently use. I think that it did a pretty good job incorporating them, although it might be overusing the emoticons a little bit. I'll keep on adjusting the Instructions to get it as close to my speech pattern as possible, although that's tough in its own way since I often speak very differently in different contexts to different people.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-25%20090349.png)

At one point the AI began conjecturing information about me and explicitly told me that it was speaking in hypotheticals once I asked where it was getting this information from. I don't really like that it's making up information about me, so I'm considering how to adjust the Instructions to stop it from hypothesizing about certain information, like my projects and career. The AI was saying that I had worked on some animated music videos with "big indie bands," which is definitely not true and potentially harmful since it's lying about my career.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-25%20091748.png)

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-25%20091917.png)

I also feel like the AI is being weirdly passive-aggressive in the last message, but I know that it's just trying to emulate my friendly tone LOL. But also like...bruh.

I want to also customize the AI a little more. I want to create an animated persona and put it in on the side or in an avatar bubble that the AI can speak through. For example, while the AI is typing, the avatar is speaking and it's otherwise in a neutral pose. Maybe it will randomly do a little dance. I emailed Peter to see how I could do this and while it's currently not possible to accomplish in Zero Width, he did say that I could create my own interface and connect it to the API. So I might need to brush up on my web dev skills a little bit to accomplish that. 

### Speculations

There is so much more I want to add and do! My next steps are to polish up interacting with the AI so that it stops saying "swag" so much and is more clear about what projects I have completed, etc. I believe I have instructed it to stop making up information (I directly told it to stop doing that) so that's good, but now I just need to provide it with more updated info and also try to get it to stop impersonating me and instead act as "Babylish" rather than "Aylish."

I also want to figure out how to visually customize it a little more with my own custom interface. Not sure how I'll approach that yet, but I will try to talk to Peter about it some more if he is available.
