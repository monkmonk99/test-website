---
layout: post
title:  "Honours Thesis"
info: "A summary of the project and a very short reflective"
tech : "AI, Python"
type: Blog
---

# My Honours Thesis

In 2023 I completed my Honours Thesis at Macquarie University. And with a pretty strong result, a high distinction, it may not have seemed like a bumpy ride. But I definitely grew a few unnoticed greys and shortened my lifespan by 6 months during those 2 semesters. It was a project that started *so* strong and with a ton of passion, but fell into a nosedive, and only at the last minute did I realise it had a relatively solid finish.

I will note here that my success is indebted to Dr Ian Wood, my supervisor, who I would consider to be rather brilliant and also a consistently easy person to converse with, even when I failed to meet expectations or blundered, as well as my family, I thank them for their tolerance of me.

## Summary

Initially, my thesis was planned to be a collaborative effort with **scambaiters** to find approximately which **social engineering** techniques work best for keeping scammers on the phone or engaged in email conversation for the longest time. This was in effort to optimise the current implementation of the [Apate project](https://apate.ai) by incorporating the results of this thesis into Apate.

The planned process for achieving this was to collect as much clean, unedited content from scambaiters as possible and train an **unsupervised** AI model to approximate on common trends and similarities between content where the scammer stays engaged for a long period of time. Specifics on this process were quite foggy and ultimately the process was blocked by lack of replies and willingness to cooperate from scambaiters.

Thus, the project pivoted to utilising **[Snorkel AI](https://www.snorkel.org/)** to classify YouTube videos on whether they are scambaiting videos or not, and additionally on the quality of the video. For our use case, we define quality as the absence of editing, interruptions, narration, and anything that obscures the conversation between the scambaiter and the scammer. 

The process for this involved first scraping data from YouTube, then transcribing the data into text, and finally using the resulting dataset from the scraped and transcribed videos as training and testing data for the model. To create a ground truth for our dataset, we utilised the **Mechanical Turk** service to provide human annotations agreed on by a census. In evaluating our model, we achieved **F1** scores of ~0.76, which we regarded as a relative success.

### Definitions

| Term               | Definition                                                                                                                                                                                                                                 |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Scambaiter         | Individuals who interact with scammers from around the world with the sole intention of agitating them and wasting their time, often as a form of content creation.                                                                        |
| Social Engineering | Specific behaviours, phrases or alike used to elicit desired reactions                                                                                                                                                                     |
| Unsupervised       | In the context of AI and machine learning, unsupervised implies the model has no guidance for what to look for and simply aims to find salient patterns. In simpler terms, the model has no true values to compare its predicted values to |
| Snorkel AI         | A platform for using human-readable heuristics as parameters in machine learning models that can classify, augment or slice datasets, with or without supervision                                                                          |
| Mechanical Turk    | A platform for paid, simple task-completion                                                                                                                                                                                                |
| F1                 | An intuitive metric for evaluating classification models                                                                                                                                                                                   |

## Reflective

My thesis had started out as a self-proposed topic between Ian and myself, with the aims of contributing to the [Apate Project](https://apate.ai), as Ian is a co-founder of the company and I had been interning as a developer for early iterations of the project in the months prior. As mentioned above, the topic was about finding the optimal social engineering techniques for scambaiting using artificial intelligence.

We set to contact, interview and request content from all the scambaiters we could. Unfortunately, we found ourselves disappointed when only one scambaiter replied, only to never reply again.  Not paying too much attention to a single obstacle, we continued with the search for scambaiters who would be willing to collaborate with us. But still no luck.
On top of this, we had begun to find far too many complications in the other steps of our plan for this current project to be considered viable. So things were looking like a dead end.

This was the beginning of a very stressful time for me. My thesis had fallen behind the recommended schedule and I was desperate to find a way to pivot my topic to something viable. My supervisor and myself finally settled on the also-above-mentioned topic of classifying scambaiting YouTube videos using machine learning based on human-readable heuristics. We had estimated that this project would be doable in our shortened project timeframe and that I would be able to utilise some of my work from our previous topic in this new topic.

The rest of the project consisted of me stressing endlessly, alternating between working furiously and procrastinating guiltily, while my supervisor monitored my progress contentedly. I suspect his lack of concern was from experiencing this process a number of times already. 

As is obvious to me now, I completed my thesis on time and with rather successful results to show for it. And while I don't consider myself overtly proud of the body of work I produced, I do consider myself proud of my demonstrated ability to manage a stressful period of my life and challenging obstacles in my career.
