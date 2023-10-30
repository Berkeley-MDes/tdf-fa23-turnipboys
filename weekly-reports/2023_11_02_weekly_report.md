# Report #10 - Week of 11/02/2023

## Aylish Turner

### Reflections

After an insightful presentation/Q&A session with Pete from ZeroWidth as well as some communication with him over Slack and email, I thought that I would try my hand at calling the ZeroWidth API through my own website.

I have website development experience, but something about this felt especially intimidating to me because I've never designed/written code for any kind of chatbot before and I don't think that I've ever actually called an API in a website before. My web dev experience is mostly just HTML/CSS/Javascript stuff for simple UI work and then implementing/embedding multimedia into the website. So this would definitely be a challenge for me, although I felt okay about approaching it in the time that I had. I guess by the end of this report we'll see if I have actually done it!

In the meantime, I realized that the way that I formatted the information for the AI's knowledge set was just...not very good at all. The AI needed much more clarity and didn't have any kind of inherent context or understanding about what I was giving it, so I knew that I would have to do a little more re-formatting and editing to make it more clear. It was especially challenging that my portfolio and LinkedIn sites are pretty out of date, so a lot of information about my recent projects isn't even already available. I had to write up a few keywords and phrases about my projects and explicitly state that they were recent projects and the AI should refer to them when asked.

I also added a new welcome message from the bot. I know that the bot cannot store information between chat sessions, but I'm curious to know what it can actively do within the chat session. So I wanted to experiment more with crafting functions. Since the AI is modeled on ChatGPT, it cannot send or take in images, which I was disappointed about. My main goal of creating a custom site for the AI to answer questions is just to see if I can create an animated avatar for the AI and make it a little more interesting when users are talking to it.

The AI also overuses a lot of the key phrases I gave it, so I have just been trying to polish up its vocabulary and speech patterns by carefully selecting the wording and instructions that I give it. It's a lot more challenging than I thought it would be and mostly a lot of manual work.

Although I uploaded my weekly reports and hoped that the context would explain itself, I did add a line telling the AI that the following text was from my weekly reports on my class projects. I had to go in and add a lot of new information manually so that the AI could make connections between the different pieces of information, especially about recent projects and classes.

After adding some new information and changing the "Intelligence" settings to pull from more than 1 item in a knowledge set, I encountered a new error warning that I hadn't seen before. It told me: "Context Window Exceeded: Your selected model has a context window of 8192 tokens. You've attempted to use 10111 tokens." I adjusted the setting down to "2" items and this resolved the issue, although I wonder if it will appear again.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-30%20143120.png)

After manually adding some information about my in-class projects, I asked the AI what some of my recent projects were. It takes a while to type out its full answer and often gives very long replies. I wonder if that is just due to the amount of information I provided it or if it has picked that up in my speech pattern information (or some third reason).

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-30%20143745.png)

The AI is VERY flattering and speaks very highly of my work, which is nice and a bit silly, but I do feel somewhat self-conscious about it. 

When I asked the AI "What are some of the games that Aylish has worked on?" it took a VERY long time to respond. I think that I might need to break up some of the information a little more. I wonder if it's too many information items? It might help to tell it to keep answers fairly short, as well.

I also keep on experiencing occasional AI "hallucinations" where it is making up information despite me directly telling it not to do that. I will try rephrasing my instructions and the order of the text to make it very clear that the AI must not make up any information about me or my projects. It's difficult to balance this because I do want it to generally also represent me, my opinions, interests, etc. on other matters.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-30%20144957.png)

I did run into the token issue again when I asked the AI: "What movie should I watch tonight? I like comedies." I guess that the best solution is probably to break up the information more or to decrease the Intelligence settings back down to just 1 item. For now, I've changed the Intelligence Knowledge Options from "Naive" to "Agentic" and kept the "Information to pull" at 2. This has fixed the issue (or so it seems) but also seems to have increased the time that it takes for the AI to reply.

Something very odd is that the AI made up information about what games I worked on again, but this time said that it CAN'T make up information that's "not present in the data [it] was trained on." So I may need to look at my instructions again to tell it to just not make anything up. However, I wonder if this would negatively affect other aspects of the AI. I also can't help but feel like it's being passive aggressive in this message even though it is literally a robot lol. I almost want to change the speech pattern to something completely different because I feel like it's triggering a negative psychological state LMAO.

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/Screenshot%202023-10-30%20150700.png)
