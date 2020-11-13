# WoC-Project-Ideas
* A list of project ideas for [Winter of Code](https://winterofcode.com/) organized by DSC-NSEC.
* Interested WoC participants can contact us on our [Discord](https://discord.gg/6vcMy5zvGD) server.

## Fake-Stream

* *Project link:* https://github.com/Nibba2018/Fake-Stream
* *Mentors:* [Soham Biswas](https://github.com/Nibba2018)

>Allows infinite streaming of a video as webcam output for different applications like Zoom, Skype etc.

**Description:** `v4l2loopback` is a kernel module which allows the creation of virtual webcams on a device running the linux kernel. The objective of `Fake-Stream` is to provide an easy to use API/SDK to modify or alter the webcam data being streamed towards that virtual camera. `FFMPEG` will be used to encode and decode such frames.

### Project Ideas
  1. **Adding audio support and generic QoL improvements:**
   So far fake stream supports video only. We would like to have the feature of streaming audio as well. Streaming of audio can be done along with the video or as a separate utility. Once audio is implemented, some Quality of Life improvements are also required(Specific details can be discussed).

      * Tech Stack: ALSA, FFMPEG and BASH.

  2. **Adding Windows Support:** Currently fake stream is available on linux only as `v4l2loopback` is a linux specific kernel module. But a work-around can be achieved using OBS virtual cams. The objective of this project would be to refactor the code to run on windows(as a separate script or as a cross platform script).

      * Tech Stack: OBS Documentation and Batch Scripting.

  3. **Adding SDK for Python or C:** Fake stream is implemented in OS specific shell scripts. Having a simple SDK will allow users to simply import fake-stream and integrate it with their own scripts or programs. For now one can work on creating sdks for Linux only.

      * Tech Stack: FFMPEG libraries for C and Python.

  4. **Pitch your own Idea!**

*Maximum Ideas to be selected for this project:* 2

## DSC-IEM Blogs

* *Project link:* https://github.com/dsc-iem/blog
* *Mentors:* [Aritra Sen](https://github.com/asrient)

### Description

Blogging for our community, a blogging website where anyone can write blogs, read, like and comment. Follow your favourite authors and get a home page with personalized suggestions

### Project Ideas

1. A detailed page for visitors traffic for every blog post. 
2. Add a footer for every page. 
3. New layout of blog items for pages like popular, trending, new arrivals. 
4. Show notifications on homepage when someone replies to your comment or likes, comments on your posts, along with a dismiss button (It should give a summary of all updates like 3 new like, 2 comments on this post etc) 
5. Check image URLs format before saving (for profile image and blog picture) 
6. Implement a way to embed items like a tweet or youtube video (oembed) 
7. Style account related pages (AllAuth pages) like forgot password, connect social accounts
8. **Pitch your own Idea!**

## rake_new2

* *Project link :* https://github.com/BALaka-18/rake_new2
* *Maintainer :* [Balaka Biswas](https://github.com/BALaka-18)

>Python library that for simple and fast keyword extraction from any text.

**Description :** `rake_new2` is a Python library that enables simple and fast keyword extraction from any text. This library works on the RAKE(Rapid Automatic Keyword Extraction) algorithm. It tries to determine the key phrases in a text by calculating the co-occurrences of every word in a key phrase and also its frequency in the entire text.

**New in v1.0.5 :**

1. Handles repetitive keywords/key-phrases

2. Handles consecutive punctuations.

3. Handles HTML tags in text : The user is allowed an option to choose if they want to keep HTML tags as keywords too.

### Project Ideas
  1. **Sentiment scoring :**
   Add sentiment scoring alongside word-degree score, to summarize emotion of the entire text based on the extracted keywords.(Specific details can be discussed)

      * Tech Stack: Python.

  2. **Spell-check feature :** Implementing automatic spell-check using NLP and Deep Learning (Specific details can be discussed).
      * Tech Stack: Python (Pre-requisite : NLP, Deep Learning, Tensorflow).

  3. **Topic Prediction module :** Add Topic prediction module in the library (Specific details can be discussed).

      * Tech Stack: Python (Pre-requisite : Deep Learning, LDA(Latent Dirichlet Allocation)).
  
  4. **Documentation  :** Writing official documentation for readthedocs.org (Specific details can be discussed).

      * Tech Stack: None (Pre-requisite : Markdown and must know/learn procedure of documentation in readthedocs.org).

  4. **Pitch your own Idea!**

*Maximum Ideas to be selected for this project:* 2