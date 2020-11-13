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

