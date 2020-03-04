Lambda Programmable Music Sequencer
===========================================

_In a short-word, [Lamu][lamu] is a Scheme interpreter with JACKAudio client as 
as a MIDI sequencer with an Lisp editor live-coding in mind._

<!--
<iframe width="560" height="315" 
src="https://www.youtube.com/embed/4Uu6bKWs_Vc" frameborder="0" 
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen>
</iframe>
-->
[![image](https://img.youtube.com/vi/4Uu6bKWs_Vc/0.jpg)](https://www.youtube.com/watch?v=4Uu6bKWs_Vc)

# Write Scheme and Make Music by Lamu #
[Lamu][lamu] (stands for LAmbda MUsic Sequencer) is a music sequencer which 
enables users to write music as Scheme programs. In this system, musical notes 
and other informations are written as Scheme's association lists. The musical 
notes can be dynamically sent to the sequencer as Scheme's association lists 
on-the-fly.  Users can also interact with the dynamically generated music at 
runtime and affect the direction that the music is going.

[Lamu][lamu] is written in Java and Scheme. It equipped with Kawa a Java based 
Scheme implementation. You can send MIDI data via JACKAudio Connection Kit a 
multiplatform audio connection system which is accessed via Java Native Access.

Lamu runs on most major platforms which can run Java such as Windows, Mac-OSX
and various Linux distributions. 

[Lamu - Lambda Programmable Music Sequencer][lamu]

# Lamu works with JACKAudio #
[JACK(JACK Audio Connection Kit)][jackaudio] is a low-latency audio framework 
which can be used in Linux,Windows and OS X. This enables a number of 
independent synthesizers, sequencers effectors to work cooperatively. The MIDI 
signals which Lamu issued are sent to the applications via JACKAudio. Lamu is 
also able to send JACKAudio commands in order to automate the 
restoring/destroying connection.

[Lamu - Lambda Programmable Music Sequencer][lamu]

# Lamu is equipped with Kawapad #
Kawapad is a Lisp editor which is written in Java. Kawapad is a customizable 
Scheme editor which is able to extend by Scheme itself. It may be a ready 
customized for editing Scheme code. It is equipped with Kawa a Scheme 
interpreter; it can execute the Scheme code on-the-fly. Kawapad is embedded in 
Lamu; though, it can run as a standalone-editor as well.

![Kawapad Editor Demo][kawapad-demo]

# Feature #
- Written in Java with JNA and runs Windows/Linux and OS X
- Built-in Kawa Scheme
- S-expressions as musical notation
- Works with JACKAudio Kit; is able to control any JACK aware Synths
- Built-in Kawapad a Lisp editor
    - is able to move around the parentheses
    - prettifies S-expressions
    - executes code blocks on-the-fly
    - can be extended by Kawa Scheme

[Lamu - Lambda Programmable Music Sequencer][lamu]

# About Me #
Lamu is invented by me and this is a single-man project. My name is Atsushi 
Oka. I am a Japanese programmer born in 1973. I was born and raised in Tokyo.  
Therefore, I have never spoken English in daily life. And as you can probably 
see, Japanese people is one of the most English resistant people.  And I am no 
exception. The grammar structure and pronunciation system in Japanese are very 
different from the rest of the world.  For Japanese people, it is extremely 
difficult to understand the difference between themselves and others.  Japan is 
geographical isolated from others; therefore, the history have been developed 
very differently.  I still haven't found the exact reason why Japanese is so 
different from others.

Therefore, you may find my documentation has some difficulty to be 
comprehended; I have to admit it and please excuse my English in advance. 

There may be something that makes me different from other Japanese; I was 
living in an extremely rural area of North-East Thailand for twelve years.  
During the time, I had encountered many accidents and happening that could lead 
me to death, but I luckily survived.  In the time, I learned a dialect of 
Laotian language and eventually I could acquire the ability to speak it very 
fluently.  That experience opened me up to other languages like English. And 
additionally I studied Scheme in the same period.

I learned Laotian music at that time and I found that it had some similarities 
with jazz. I was a jazz guitarist.  I have been inquiring to find the way to 
mix jazz, Laotian music and other music for decades. And I hope someday I can 
develop a whole new type of music.

Less have I visited to English spoken countries; I have visited to Boston, 
Massachusetts back in 1996 for only three month and 2002 for only a month. My 
English ability is quite limited. Please, excuse my English and thank you for 
your corporation to be patient to the immatureness.


[jackaudio]: https://jackaudio.org/
[kawapad-demo]: https://lambda-music.github.io/lamu/imgs/corresponding-parenthesis-movement.gif
[lamu]:  https://lambda-music.github.io/lamu/
[kawapad]: https://lambda-music.github.io/lamu/workspace/kawapad/
[architecture]: https://lambda-music.github.io/lamu/imgs/lambda-music-architecture.png
[vim-modeline]: # ( vim: set spell expandtab fo+=aw: )
