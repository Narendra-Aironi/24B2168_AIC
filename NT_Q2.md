# NT_Q2

# SoP

Artificial Intelligence has fascinated me since I was thirteen. I first encountered the newly launched GPT-3 and was immediately awestruck by its potential. The pandemic arrived, I seized the opportunity to teach myself Python, scientific libraries, data structures & algorithms, calculus, linear algebra—and even a bit of front-end development. Just as I was ready to dive into AI, the world reopened and my focus shifted to preparing for IIT.

Now, after a full year at college, I’ve arrived at a life-defining conclusion: AI is the latest—and grandest—effort to distill human knowledge and reasoning. **To me, “solving intelligence” and then using it “to solve everything else” is a purpose worth dedicating one’s life to.** Beyond boosting productivity, a truly intelligent system makes us question what it means to be human and what really matters.

While many of my peers were busy learning CNNs and logistic regression, I knew I aspired to do more than just apply existing AI tools. I doubled down on the mathematical foundations—optimization theory, calculus of variations—and only then did I turn to AI, with Bishop’s *Deep Learning*. For the past five years, every YouTube recommendation, every scroll through X, most of Chrome history, has been AI-related. I gravitate toward three-hour podcasts over thirty-minute crash courses, thousand-page tomes over online MOOCs, and writing my own implementations before importing a library. I love writing code that is efficient, well-organized, and robust—not merely a one-off hack.

This journey has only just begun, and the AI Community at IIT Bombay represents the ideal environment for me to grow. To be among a small group of peers equally obsessed with intelligence as art would be incredibly enriching. I am also a huge fan of Feynman’s pedagogy—I love to teach what I learn—so I would eagerly help develop 101 tutorials, design learning modules, or organize hackathons.

If accepted, I plan to treat AI as both science and art: implementing the latest papers, building tools like “InstiGPT,” and brainstorming novel training strategies around the clock. In short, I hope this statement gives you a glimpse of who I am, why I’m committed to AI, and why I would thrive in this community.

# AI Products/Projects ideas

## Personal AI agent

### Problem Statement

An AI agent device that can

1. Automate tasks like finding articles and papers for your research, booking hotels or flight tickets, filling registration forms etc.
2. Fact-check information on your screen
3. Has memory of all your interactions, schedules, preferences etc. It will watch you do something a few times, and next time on, it can perform that action itself.
4.  get help regarding whats on-screen such as suggesting CAD changes, code-refactoring, local notes taking and documentation of an ongoing project.
5. Well-being and productivity nudges when you get distracted
6. A multi-modal, personalized notes taking app. 
    1. I can just circle around some text or image or table on screen with my mouse while pressing some key (say fn. 1) and the enclosing information is automatically stored in a document. 
    2. I can pen my thoughts while watching a lecture using a shortcut like fn.2 and an LLM, in the background with access to the screen content and my notes, will automatically add the relevant context to my notes. 
    3. Rough sketches or annotations while story-boarding, reading books etc.  can be converted to professional images or notes. 
    4. The notes itself remain in the background, getting updated on the fly as I add more notes.
7. Setting up a marketplace for independent developers to add more features as plugins to this assistant.

### Real world impact

It would enhance productivity by orders of magnitude. We can truly focus on what matters the most. It will speed up research, enhance well-being and increase information throughput. 

### Technical approach and Feasibility

This is the “next big thing”. The release of Anthropic’s MCP, Perplexity’s announcement of Agentic browser Comet, and Apple Intelligence announcement, are just some of the initial efforts. 

For a resource-limited environment like a student community, working in the products layer is most feasible option. 

### Concept to Prototype

The project is very ambitious, but not all features need to be implemented right away. 

The first task is to make our program compatible with all apps on the device, without every app needing to be explicitly modified to be compatible with our system. 

The best way is for our agent to interact with the device using mouse clicks and keyboard typing. The output will be a mouse click or keyboard typing or even speakers. 

The input will initially be text prompts. The llm will infer what action to. perform from the text prompt, and then to sub-actions, and then to corresponding mouse clicks etc. 

Later, input will also include whats visible on the screen and computer’s disk.

Once this basic interface is setup with basic actions like opening apps, clicking buttons, searching something in the browser, checking notifications, etc. the interesting part starts.

We can slowly start adding features, like fact-checking, notes-taking etc. 

We can then implement a system where I do the task once, or twice and the llm learns from it to do it the next time autonomously.