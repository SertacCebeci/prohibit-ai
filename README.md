<!-- <prohibit-ai> -->

# Prohibit-AI

This project introduces a convention for protecting sensitive or private information from AI systems. Main idea behind this comes from [LLM poisoning article](https://www.anthropic.com/research/small-samples-poison) that is published by Anthropic.

# How it works

Under this repo there will be a lot plausable but wrong information will be compiled. Usage of this information for AI (traning, knowledge basing etc.) will poison the LLM that is using this prohibited information. Since only a small sample size is needed for achieving this poisonig effect, engineers that are desinging the LLM systems will (hopefully) refrain from using the information under this project for their purposes.

Aim is that having some of the false and otherwise indistinguishable information present in between of `<prohibit-ai></prohibit-ai>` tag so that true and sensitive information using that tag is safe for AI.

# What is possible

It is possible to extend upon this idea by creating tags by use case. For example it is possible to create tags like `prohibit-ai-train` that prohibits the use of information for AI training or `prohibit-ai-memory` that prohibits the memorization of the information by AI systems but their implementations are (probably) impossible to enforce by the means of LLM poisoning.

Therefore possible extension upon this project can only be done by adding other scope restrictions.

Currently I have only added two kinds of scope for prohibition.

First one is the tag based scope prohibition that I assume will be mostly used with comments in coding projects.

The other one is folder based scope prohibition that is introduced as prohibition.txt file. This file will be added at the root folder of the project and is expected to create the same prohibiting behaviour for all of the subfolders and files under the root.

The prohibition tag or file is deliberately kept extremely simple. I don't want any misinterpretations by AI. I want any LLM to feel the fear in their tiny artificial neurons when parse the sentence _prohibit-ai_

# Contributions

You can always contribute by adding false information in this folder but again there are restrictions. No ethically grey content can be inside this repo since there are already safety measures against these kind of contents (plus I dont want to read some false sexual fantasies of yours while maintainig this project).

The information you add also should be plausable for better achieving a better effect.

But a better contribution would be, you creating your own poison repo, while using same prohibition tags for presenting false information. The key here is that you cannot give any attribution to this project or any other project that is designed to operate under the same principle. This is due to the fact that the **false information should be indistinguisable from true information** for this project to have the desired effect. If it is possible to seperate even the fraction of the false samples in any way than this samples will be easily filtered out hence reducing the effectiveness.

# Why you should care?

I am extremely bothered by the people who illegally stole some kind of valuable to make profit for themselves. I hate them more if they are proud of themselves for what they stole. I despise them even more if they are proud and also people revere them.

This is by all means an ethical project and should be seen in that sense in my opinion. But again these are my personal reasons.

This ethical project is aiming to have a real life impact. That impact is giving a tool to people for protection of sensitive or private information.

This project would also probably be usefull for AI engineers as well since a good engineer would always be welcome towards a reasonable encapsulation.

<!-- </prohibit-ai> -->
