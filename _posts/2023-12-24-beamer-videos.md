---
layout: post
title: Embedding videos in beamer
date: 2023-12-09 08:51:00-0400
description: Adding videos to latex presentations
tags: formatting
categories: 
related_posts: false
---

Ever since flash is not supported by pdfs you need to do a bit more work to get videos to work. 
Federico Tartarini made this very nice bit of code to include videos in your latex beamer presentations
[Embed video](https://gist.github.com/FedericoTartarini/7af4eb6fc13b1cb9cc68b7e8ea823d50)

````
\documentclass[12pt,a4paper]{beamer}
\usepackage[latin1]{inputenc}
\input{embed_video.tex}

\begin{document}

\begin{frame}{Example}

\begin{figure}
\embedvideo{\includegraphics[width=7cm]{./Pictures/screen_shot.png}}{./Movies/Movie.mp4}
\caption{Click to play}
\end{figure}
\end{frame}

\end{document}

`````
