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

## Python Reverse Shell

* *Project link:* https://github.com/whokilleddb/Reverse-Shell
* *Mentors:* [Debjeet Banerjee](https://github.com/whokilleddb/Reverse-Shell)

>Reverse Shell For Command And Control with Extended Functionality

**Description:**  A [standard reverse shell](http://pentestmonkey.net/cheat-sheet/shells/reverse-shell-cheat-sheet) in python is mostly limited to primitive command execution. Often, a simple STDERR can terminate the remote session, which isn't a favourable scenario for a hacker. Here, the aim is to provide a more stable C&C framework.

### Project Ideas
  1. **Adding Encryption:**
   So far, the program doesn't have an encryption method for outgoing/incoming byte streams. An added layer of encryption would be instrumental in preventing detection by AV engines.

      * Tech Stack: Python

  2. **Adding Persistence:**
   Adding persistence by creating executables or as scripts to trigger the program at runtime.

      * Tech Stack: Bash, Batch, Python.

  3. **Add Keylogging And Webcam Hijack Modules:** 
   Add Keylogging and Webcam hijack functionalities which run on a different thread (not along the main thread).

      * Tech Stack: Python.

  4. **Automated Recon :** 
   An automated script to gather system information and perform auto recon on potential attack vectors which can be gathered from websites like (Gtfobin)[https://gtfobins.github.io/].

      * Tech Stack: Python.

  4. **Pitch your own Idea!**

*Maximum Ideas to be selected for this project:* 2

## DSC-IEM Blogs

* *Project link:* https://github.com/dsc-iem/blog
* *Mentors:* [Aritra Sen](https://github.com/asrient) & [Mahak Makharia](https://github.com/mahakmakharia)

### Description

Blogging for our community, a blogging website where anyone can write blogs, read, like and comment. Follow your favourite authors and get a home page with personalized suggestions

### Project Ideas

1. **Visitors traffic page** A detailed page for visitors traffic for every blog post, the visitors count button on the blog page should take you to this page, only visible to the blog author. This page should list out `total visits`, `unique visits`, `visits this week`, `avg duration of a visit`, `top referer sites`, all these information can be derived or computed from `View` model of our database which is already implemented. You need to work on both backend and frontend, extract the values from the db and design the webpage showcasing the values.
    * Tech Stack: Python, Django, HTML, CSS
    
2. **Notifications** Show notifications on homepage when someone replies to your comment or likes, comments on your posts, along with a dismiss button (It should give a summary of all updates like 3 new like, 2 comments on this post etc). A notification should be shown only once. To keep track of what notifications to show and dismiss, create a new db model called `Alerts` or similar, one possible implementation maybe: `user`: the one who will receive the notif, `type`: eg `blog.likes`, `blog`: reference blog post or `None`,`ref_user`: reference to the user who caused it or `None` eg: when user5 liked your post, blog will be ref to the post, and user will be yourself i.e author and ref_user will be user5. Again when someone follows you, blog will be set to None, ref_user will be the follower. Every time something happens like a follow, or like or comment a notif will be generated and a summary of all the notifications will be generated and shown to the user on their homepage. You may also create a separate detailed page for notifications along with the homepage banner if time permits.
    * Tech Stack: Python, Django, HTML, CSS
 
3. **Embedding youtube videos** Implement a way to embed youtube videos (oembed). Twitter, youtube and many others provide a way to embed their content into a webpage, called oembed. We dont allow authors to use iframes directly into their post and the embed html code that they provide is an iframe. We need to implement something like this module [pyembed-markdown](https://github.com/pyembed/pyembed-markdown) You can use this as a reference. We are not using this modules because it is not maintained anymore also it has some bugs that cause parsing youtube links too much time-consuming. We plan to parse the ombed links on the client side to reduce loading time. We can implement some apis that will take a youtube link and parse it to its appropriate html, once we get the html of each link we replace the links with the html on the client-side. We can ask the author to embed a youtube video like `{yt}(link to the video)` or similar and once the page is loaded, we look for such patterns and convert each of them to their html.
    * Tech Stack: Python, JavaScript, jQuery

4. **Pitch your own Idea!**

*Maximum Ideas to be selected for this project:* 2

## Text Sentiment Analysis

* *Project link:* https://github.com/khanfarhan10/TextSentimentAnalysis
* *Mentors:* [Farhan Hai Khan](https://github.com/khanfarhan10) & [Tannistha Pal](https://github.com/paltannistha)

### Description

Text Sentiment Analysis in Python using Natural Language Processing (NLP) for Negative/Positive Content Detection and further classification accordingly to Overwhelming Speech, Appreciation Speech, Demoralising Speech and Hate Speech. Deployed on the Cloud using Streamlit on the Heroku Platform.

### Project Ideas

1. Add models with higher accuracies than the basic and intermediate ones provided with deployment (preferred : tensorflow 2.x, keras & pytorch DNNs). 
      * Tech Stack: Python Deep Learning with NLP - Keras, Tensorflow , Pytorch etc.
2. Better UI with customized look (in Flask). 
      * Tech Stack: Python Flask with HTML5 & CSS3 for Frontend Support.
3. Better utility tools for uploading a zipfile and getting an excel sheet with a workbook of respective txt files etc. 
      * Tech Stack: Python Zipfile Handling, Pandas & Numpy.
4. More analysis based improvement such as decorating nouns, verbs, etc. 
      * Tech Stack: Python Core NLP : Training on Datasets.
5. Providing utility applications such as summarization, paraphrasing etc. 
      * Tech Stack: Python Utilities with NLP.
6. Deploy to an Android App (Flutter).
      * Tech Stack: Android Studio, Dart with Flutter.
7. **Pitch in your own Innovative Ideas!**  
*Maximum Ideas to be selected for this project:* 3
## rake_new2

* *Project link :* https://github.com/BALaka-18/rake_new2
* *Mentors :* [Balaka Biswas](https://github.com/BALaka-18) & [Aanisha Bhattacharya](https://github.com/Aanisha)

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
