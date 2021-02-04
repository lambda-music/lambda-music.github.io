*In a short-word, [Lambda Music Sequencer][LNK_LAMU] is a Scheme interpreter 
with JACKAudio client as as a MIDI sequencer with an Lisp editor live-coding in 
mind.*

<iframe id="main-video" style="width:100%;"
src="https://www.youtube.com/embed/4Uu6bKWs_Vc" frameborder="0" 
allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen>
</iframe>
<script>
window.addEventListener( 'load' , function() {
    var e = document.getElementById( 'main-video' );
    e.style.height = (e.offsetWidth * 0.5625) + 'px';
});
</script>
<!--
[![image](https://img.youtube.com/vi/4Uu6bKWs_Vc/0.jpg)](https://www.youtube.com/watch?v=4Uu6bKWs_Vc)
-->

# Write Scheme and Make Music by Lamu #
[Lamu][LNK_LAMU] (stands for LAmbda MUsic Sequencer) is a music sequencer which 
enables users to write music as Scheme programs. In this system, musical notes 
and other informations are written as Scheme's association lists. The musical 
notes can be dynamically sent to the sequencer as Scheme's association lists 
on-the-fly.  Users can also interact with the dynamically generated music at 
runtime and affect the direction that the music is going.

[Lamu][LNK_LAMU] is written in Java and Scheme. It equipped with Kawa a Java 
based Scheme implementation. You can send MIDI data via JACKAudio Connection 
Kit a multiplatform audio connection system which is accessed via Java Native 
Access.

Lamu runs on most major platforms which can run Java such as Windows, Mac-OSX
and various Linux distributions. 

[Lamu - Lambda Programmable Music Sequencer][LNK_LAMU]

# Lamu works with JACKAudio #
[JACK(JACK Audio Connection Kit)][jackaudio] is a low-latency audio framework 
which can be used in Linux,Windows and OS X. This enables a number of 
independent synthesizers, sequencers effectors to work cooperatively. The MIDI 
signals which Lamu issued are sent to the applications via JACKAudio. Lamu is 
also able to send JACKAudio commands in order to automate the 
restoring/destroying connection.

[Lamu - Lambda Programmable Music Sequencer][LNK_LAMU]

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

[Lamu - Lambda Programmable Music Sequencer][LNK_LAMU]

[jackaudio]: https://jackaudio.org/
[kawapad-demo]: https://lambda-music.github.io/lamu/imgs/corresponding-parenthesis-movement.gif
[LNK_LAMU]: https://lambda-music.github.io/lambda-music/
[EDT_LAMU]: ../lamu/readme.md
[kawapad]: https://lambda-music.github.io/lamu/workspace/kawapad/
[architecture]: https://lambda-music.github.io/lamu/imgs/lambda-music-architecture.png

