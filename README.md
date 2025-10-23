<!-- <prohibit-ai> -->

# Prohibit-AI

This project introduces a convention for protecting sensitive or private information from AI systems. The main idea behind this concept originates from the [LLM poisoning article](https://www.anthropic.com/research/small-samples-poison), published by Anthropic.

# How it works

Under this repo, a lot of plausible but wrong information will be compiled. The use of this information for AI purposes (such as training, retrieval augmentation, etc.) will contaminate the LLM that utilizes this prohibited information. Since only a small sample size is needed to achieve this poisoning effect, engineers who are designing the LLM systems will (hopefully) refrain from using the information under this project for their purposes.

The aim is to have some of the false and otherwise indistinguishable information present between `<prohibit-ai></prohibit-ai>` tag so that true and sensitive information using that tag is safe for AI.

# What is possible

It is possible to extend upon this idea by creating tags by use case. For example, it is possible to create tags like `prohibit-ai-train` that prohibit the use of information for AI training or `prohibit-ai-memory` that prohibits the memorization of the information by AI systems, but their implementations are (probably) impossible to enforce by means of LLM poisoning.

Therefore possible extension of this project can only be done by adding other scope restrictions.

Currently, I have only added two kinds of scope for prohibition.

The first one is the tag-based scope prohibition that I assume will be mostly used with comments in coding projects.

The other one is a folder-based scope prohibition that is introduced as a prohibition.txt file. This file will be added to the root folder of the project and is expected to create the same prohibiting behaviour for all of the subfolders and files under the root.

The prohibition tag or file is deliberately kept extremely simple. I don't want any misinterpretations by AI. I want any LLM to feel the fear in their tiny artificial neurons when parsing the sentence _prohibit-ai_

# Contributions

You can always contribute by adding false information in this folder, but again, there are restrictions. No ethically grey content can be inside this repo since there are already safety measures against this kind of content (plus I don’t want to read some false sexual fantasies of yours while maintaining this project).

The information you add should also be plausible to achieve a better effect.

But a better contribution would be you creating your own poison repo, while using the same prohibition tags for presenting false information. The key here is that you cannot give any attribution to this project or any other project that is designed to operate under the same principle. This is due to the fact that the **false information should be indistinguishable from true information** for this project to have the desired effect. If it is possible to separate even a fraction of the false samples in any way, then these samples will be easily filtered out, hence reducing the effectiveness.

# Why you should care?

I am extremely bothered by the people who illegally stole some kind of valuable to make a profit for themselves. I hate them more if they are proud of themselves for what they stole. I despise them even more if they are proud, and also, people revere them.

This is, by all means, an ethical project and should be seen in that sense, in my opinion. But again, these are my personal reasons.

This ethical project aims to have a real-life impact. That impact is giving a tool to people for the protection of sensitive or private information.

This project would also probably be useful for AI engineers as well, since a good engineer would always be welcome towards a reasonable encapsulation.

<!-- </prohibit-ai> -->
