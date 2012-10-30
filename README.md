# ub-beamer

Beamer template inspired by the corporate design of the University of Bamberg

## Usage

Include the `ub-beamer.sty` file in your path and use it with a `\usepackage` command.
You also need the pdf file `images/ub-logo.pdf` that contains the logo image to be used on the slides.

Simple usage scenario, also contained in `example.tex`:

```tex
\documentclass{beamer}
\usepackage{ub-beamer}

%Meta information
\title{Template for a Beamer Presentation using the University of Bamberg Corporate Design}
\author{J\"org Lenhard}
\institute{Distributed Systems Group - WIAI - University of Bamberg}
\date{\today}

%The content of the slides
\begin{document}

\begin{frame}[plain]
	\titlepage
\end{frame}

\begin{frame}{Title of the slide}
This is a template for a University of Bamberg presentation with beamer
\end{frame}

\end{document}
```
	
## Features
The template comes with the following color definitions that conform to the University of Bamberg colors

	UBBlue
	UBBlack
	UBYellow
	UBGreen
	UBRed
	UBGray
	
It offers several commands for formatting text in blue 

```tex
%Marks text in blue
\markB{some text}
 	
%Marks text in blue and bold
\markBB{some text}
 	
%Marks text in blue and italic
\markBI{some text}
```
 	
You can use another logo next to the university logo (your group logo) by redefining a variable.
This logo will show up in the right upper corner of each slide instead of the university logo.

```tex
\def \grouplogofile {images/example-group-logo.pdf}
```
	
The template uses square bullet points instead of round ones.