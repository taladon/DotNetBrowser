# DotNetBrowser

This project is to create a fully managed .NET browser implementation that can run on Windows, Linux, MacOs, and anything else that can run .NET.

# Are you nuts? It would take years and tons of man-hours!

The way I see things, those are excuses rather than legitimate reasons not to do this. We go to the moon not because it's easy, etc. I realize the scope of this project, and that it's going to take more than me to get it done. I'm doing this partly to learn, and partly because I hope someday this may be useful to other people. My philosophy is to go forth boldly, so that's what I'm doing.

There are two large pieces that I'm still researching. I don't intend to write a javascript interpreter or whatever is needed to run WebAssembly. If possible, the plan is to integrate an existing javascript engine (maybe allow the user to choose a javascript engine). I need to research WebAssembly more to know what options are possible.

# Ok, so what's the plan? Are you starting totally from scratch?

I thought about starting from scratch and was prepared to do so. Then I found https://github.com/ArthurHub/HTML-Renderer which is a .NET Html Renderer. From the README, it currently targets HTML 4.01 and CSS level 2 specifications support. This is a great starting position, since there is css parsing, image loading, and a DOM. Currently my plan is to add HTML 5 rendering support, then start making the code more browser-like. (This includes things like adding a caching mechanism, handling cookies, file downloads, etc).

# Why this isn't a fork of ArthurHub/HTML-Renderer

The main advantage of making this project a fork would be to submit enhancements upstream. The main issue I see is that making this a full web browser is going to be such a rework that people who use the ArthurHub project would have to change their code significantly to use this project. Also, the ArthurHub project hasn't had much activity in a long time. When possible, I will manually submit PR's to ArthurHub, especially in the beginning as I fix bugs / enhance the rendering portion.

# Current Status

Currently, everything compiles and at least runs. The WPF Demi application is the one I started updating. There is a textbox to enter url's and a go button that navigates to the page. There is currently no history, bookmarks, etc. 

I'm currently evaluating the existing codebase and working on setting up overall structures for the various browser features. I'm also working on updating the demo application to be more useful.

# How you can help

 If you're interested in helping, PR's are welcome. However, the first priority is to get the architecture right. Once it's posted, feel free to comment, make suggestions, etc.

# How to contact me

 I have a regular full time job, but I can get on any of the major chat platforms in the evenings if you'd like to have a deeper conversation. I can also be reached via email -- taladon at gmail dot com