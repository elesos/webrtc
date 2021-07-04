# FAQ




### Why should I use WebRTC?

We think you'll want to build your next video-chat style application using
WebRTC. Here's why:

  * A key factor in the success of the web is that its core technologies --
    such as HTML, HTTP, and TCP/IP -- are open and freely implementable.
    Currently, there is no free, high-quality, complete solution available
    that enables communication in the browser. WebRTC enables this.

  * Already integrated with best-of-breed voice and video engines that have
    been deployed on millions of endpoints over the last 8+ years. Google does
    not charge royalties for WebRTC.

  * Includes and abstracts key NAT and firewall traversal technology, using
    STUN, ICE, TURN, RTP-over-TCP and support for proxies.

  * Builds on the strength of the web browser: WebRTC abstracts signaling by
    offering a signaling state machine that maps directly to `PeerConnection`.
    Web developers can therefore choose the protocol of choice for their usage
    scenario (for example, but not limited to, SIP, XMPP/Jingle, et al.).


### What is the Opus audio codec?

[Opus][opus-link] is a royalty-free audio codec defined by IETF
RFC 6176.  It supports constant and variable bitrate encoding from 6 kbit/s to
510 kbit/s, frame sizes from 2.5 ms to 60 ms, and various sampling rates from
8 kHz (with 4 kHz bandwidth) to 48 kHz (with 20 kHz bandwidth, where the
entire hearing range of the human auditory system can be reproduced).

[opus-link]: http://opus-codec.org/

### What is the iSAC audio codec?

iSAC is a robust, bandwidth-adaptive, wideband and super-wideband voice codec
developed by Global IP Solutions, and is used in many Voice over IP (VoIP) and
streaming audio applications. iSAC is used by industry leaders in hundreds of
millions of VoIP endpoints. This codec is included as part of the WebRTC
project.


### What is the iLBC audio codec?

iLBC is a free narrowband voice codec that was developed by Global IP
Solutions, and is used in many Voice over IP (VoIP) and streaming audio
applications. In 2004, the final IETF RFC versions of the iLBC codec
specification and the iLBC RTP Profile draft became available. This codec is
included as part of the WebRTC project.


### What is the VP8 video codec?

VP8 is a highly-efficient video compression technology developed by the WebM Project. It is the video codec included with WebRTC.

### What is the VP9 video codec?

Similar to VP8, VP9 is also from the WebM Project. Its a next-generation open video codec. From Chrome 48 on desktop and Android, VP9 will be an optional video codec for video calls. More details in [Google Developers][vp9-link].

[vp9-link]: https://developers.google.com/web/updates/2016/01/vp9-webrtc/

### What other components are included in the WebRTC package?

#### Audio

WebRTC offers a complete stack for voice communications. It includes not only
the necessary codecs, but other components necessary to great user
experiences. This includes software-based acoustic echo cancellation (AEC),
automatic gain control (AGC), noise reduction, noise suppression, and
hardware access and control across multiple platforms.


#### Video

The WebRTC project builds on the VP8 codec, introduced in 2010 as part of the
[WebM Project][webm-link]. It includes components to conceal
packet loss and clean up noisy images, as well as capture and playback
capabilities across multiple platforms.

[webm-link]: http://www.webmproject.org/

#### Network

Dynamic jitter buffers and error concealment techniques are included for audio
and video, which help mitigate the effects of packet loss and unreliable
networks. Also included are components for establishing a peer-to-peer
connection using ICE / STUN / Turn / RTP-over-TCP and support for proxies.



### How can I test the quality of WebRTC components?

We have put sample applications [here][examples-link].

[examples-link]: https://webrtc.googlesource.com/src/+/refs/heads/master/docs/native-code/development/index.md#example-applications


### Are WebRTC components subject to change?

WebRTC is based on a API that is still under development through efforts at
WHATWG, W3C and IETF. We hope to get to a stable API once a few browser
vendors have implementations ready for testing. Once the API is stable, our
goal will be to offer backwards compatibility and interoperability. The WebRTC
API layer will be our main focus for stability and interoperability. The
components under it may be modified to improve quality, performance and
feature set.


### WebRTC components are open-source. How do I get the source and contribute code?

Please see [Getting Started][getting-started-link] and
[Contributing bug fixes][contributing-link] for more information.

[getting-started-link]: https://webrtc.googlesource.com/src/+/refs/heads/master/docs/native-code/development/index.md
[contributing-link]: https://webrtc.org/support/contributing


### To be a Contributor, do I need to sign any agreements?

Yes, each Contributor must sign and return the
[Contributor License Agreement][cla-link]

[cla-link]: https://developers.google.com/open-source/cla/individual?hl=en


### Do I have to be a programmer to use WebRTC?

Yes, to build WebRTC support into a software application or contribute
improvements, programming skills are required. However, usage of the
JavaScript APIs that call WebRTC in the browsers will only require typical web
development skills.




### Are the WebRTC components from Google's acquisition of Global IP Solutions?

Yes. Some components, such as VoiceEngine, VideoEngine, NetEQ, AEC, et al. all
stem from the GIPS acquisition收购.


### What codecs are supported in WebRTC?

The currently supported voice codecs are G.711, G.722, iLBC, and iSAC, and VP8
is the supported video codec. 


### Please explain how WebRTC is free of charge?

Some software frameworks, voice and video codecs require end-users,
distributors and manufacturers to pay patent royalties to use the intellectual
property within the software technology and/or codec. Google is not charging
royalties for WebRTC and its components including the codecs it supports (VP8
for video and iSAC and iLBC for audio).  For more information, see the [License
page][license-link].

[license-link]: https://webrtc.googlesource.com/src/+/refs/heads/master/docs/license/index.md








### What if someone gets the code from Google and gives it to me without changes. Do I have a patent grant from Google?

Yes, you still have the right to redistribute and you still have a patent
license for Google's patents that cover the code that Google released.


### What if someone makes a change to the code and gives it to me. Do I have a patent license from Google for that change?

You still have the right to redistribute but no patent license for the changes
(if there are any patents covering it). We can't give patent licenses for
changes people make after we distribute the code, as we have no way to predict
what those changes will be. Other common licenses take the same approach,
including the Apache license.


### What if Google receives or buys a patent that covers the code I receive sometime after I receive the code. Do I have a patent grant for that patent?

Yes, you still have the right to redistribute and you still have a patent
license for Google's patents that cover the code that Google released.


### What if my competitor uses the code and brings patent litigation against me for something unrelated to the code. Does he or she still have a patent license?

Yes, he/she still has the right to redistribute and he/she still has a patent
license for Google's patents that cover the code that Google released.
