---
layout: post
title: Embedding videos in beamer
date: 2023-12-24 08:51:00-0400
description: Adding videos to latex presentations
tags: latex
categories: formatting
related_posts: false
---

Flash is not supported anymore by Adobe so you need to do a bit more work to get videos to work in latex. 
Federico Tartarini made this very nice bit of code to include videos in your latex beamer presentations
[Embed video](https://gist.github.com/FedericoTartarini/7af4eb6fc13b1cb9cc68b7e8ea823d50) Put the .tex in the same folder as your main document. You can then use the code below to include a video in your presention: 

````
\documentclass[12pt,a4paper]{beamer}
\usepackage[latin1]{inputenc}
\input{embed_video.tex}

\begin{document}

\begin{frame}{Example}

\begin{figure}
\embedvideo{\includegraphics[width=7cm]{./Pictures/screen_shot.png}}{./Movies/Video.mp4}
\caption{Click to play}
\end{figure}
\end{frame}

\end{document}

`````

A notable workaround was using ``\usepackage{multimedia}`` with Foxit.  However, Foxit has also stopped supporting flash.  