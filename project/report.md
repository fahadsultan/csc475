

# Report 

## Project Title 
Come up with a good title for your project.

## Author Information 
Should include your name and email address in the author description. 

## Abstract
The abstract should be a concise summary of the entire report. It should include a brief description of the problem, the methods used, and the results. It should be no more than 200 words.


## Introduction

_A lot of the first half of the introduction should come from the proposal._

Your introduction section should set the scene for the report by describing what problem you are attempting to solve, or what knowledge you are hoping to discover. Describe in detail motivations of the problem. Why is it important or interesting? What are the consequences of not solving it? Include statistics related to the problem to argue why the problem needs attention and cite their source(s) e.g. "Dietary increase in glucose consumption over the past 100 years has led to a national epidemic of type 2 diabetes" [1] Connect it to some of the issues we have discussed in class, if relevant, citing the relevant readings. 


State your proposed solution to the problem.
Briefly motivate why you chose this goal -- why do you think it is important, interesting, challenging and/or likely to succeed?
If you have any secondary or stretch goals (i.e. things you will do if you have time), please also describe them. Describe the task clearly -- give an example of an input and an output, if applicable.


In the second half of the introduction, briefly summarize the rest of the report, making sure to include a few sentences on each of the following section: Data, Methods and Preliminary Results. 


## Related Work
Include literature review here.

## Data


\begin{figure}[h]
\centering
\includegraphics[width=.8\textwidth]{figures/map.png}
\caption{Spatial distribution of data}
\label{fig:pipeline}
\end{figure}

Describe in detail the data set you use in your project. Broadly explain the organization of the data and the information it contains.

Start off by stating the source of the data, who collects the data and with what frequency. If the data is publicly available, cite the source. 

Make sure to state your sample size: N i.e. the number of observations (rows).

What are the features (columns)? Create a table, if possible. For data sets with too many features to include in a table, describe the 'categories' or the general nature of the features. 

What is the time range and resolution of the data? What is the geographic/spatial range and resolution of the data?

Do you filter out any rows? If so, why? Do you aggregate any rows? If so, explain why and how. 

State any potential limitations, biases, anomalies, or other issues with the data.

| Country Name or Area Name | ISO ALPHA 2 Code | ISO ALPHA 3 Code | ISO numeric Code |
|---------------------------|------------------|------------------|------------------|
| Afghanistan               | AF               | AFG              | 004              |
| Aland Islands             | AX               | ALA              | 248              |
| Albania                   | AL               | ALB              | 008              |
| Algeria                   | DZ               | DZA              | 012              |
| American Samoa            | AS               | ASM              | 016              |
| Andorra                   | AD               | AND              | 020              |
| Angola                    | AO               | AGO              | 024              |


_Have at least one figure for the data section that highlights some essential property of the data. These are generally histograms. If your data has a time column, you might want to consider adding a line plot here. If the data has a spatial column, maybe add a map._


## Methods

```{figure} figures/pipeline.png
---
height: 50%
name: directive-fig
---
Pipeline of the project
```


Describe the methods you used to solve the problem. 

_Include at least a schematic of the general pipeline from Data Collection or Preprocessing, followed by Analysis / Models and Finally Outcome._

Explain in detail each piece of the pipeline, making sure to include any equations or algorithms you use. Mention and cite any libraries or frameworks you use. 

Finally, add a link to your GitHub repository to direct to the reader to your code implementing the methods in case the reader wants to reproduce or expand the results. 



\begin{algorithm}[h]
\caption{An algorithm with caption}\label{alg:cap}
\begin{algorithmic}
\Require $n \geq 0$
\Ensure $y = x^n$
\State $y \gets 1$
\State $X \gets x$
\State $N \gets n$
\While{$N \neq 0$}
\If{$N$ is even}
    \State $X \gets X \times X$
    \State $N \gets \frac{N}{2}$  \Comment{This is a comment}
\ElsIf{$N$ is odd}
    \State $y \gets y \times X$
    \State $N \gets N - 1$
\EndIf
\EndWhile
\end{algorithmic}
\end{algorithm}


## Results


% \begin{figure}[h!]
%     \centering
%     \includegraphics[width=.3\textwidth]{figures/results.jpeg}
%     \caption{Results figure}
%     \label{fig:enter-label}
% \end{figure}

\begin{figure}
     \centering
     \begin{subfigure}[b]{0.3\textwidth}
         \centering
         \includegraphics[width=\textwidth]{figures/results.jpeg}
         \caption{$y=x$}
         \label{fig:y equals x}
     \end{subfigure}
     \hfill
     \begin{subfigure}[b]{0.3\textwidth}
         \centering
         \includegraphics[width=\textwidth]{figures/results.jpeg}
         \caption{$y=3\sin x$}
         \label{fig:three sin x}
     \end{subfigure}
     \hfill
     \begin{subfigure}[b]{0.3\textwidth}
         \centering
         \includegraphics[width=\textwidth]{figures/results.jpeg}
         \caption{$y=5/x$}
         \label{fig:five over x}
     \end{subfigure}
        \caption{Three simple graphs}
        \label{fig:three graphs}
     \begin{subfigure}[b]{0.3\textwidth}
         \centering
         \includegraphics[width=\textwidth]{figures/results.jpeg}
         \caption{$y=x$}
         \label{fig:y equals x}
     \end{subfigure}
     \hfill
     \begin{subfigure}[b]{0.3\textwidth}
         \centering
         \includegraphics[width=\textwidth]{figures/results.jpeg}
         \caption{$y=3\sin x$}
         \label{fig:three sin x}
     \end{subfigure}
     \hfill
     \begin{subfigure}[b]{0.3\textwidth}
         \centering
         \includegraphics[width=\textwidth]{figures/results.jpeg}
         \caption{$y=5/x$}
         \label{fig:five over x}
     \end{subfigure}
        \caption{Three simple graphs}
        \label{fig:three graphs}
\end{figure}


\begin{table}[b]
\centering
\caption{An important Results table}
    \begin{tabular}{|c|l|S|S|S|S|}           \hline 
\multirow{2}{*}{\# of class} &\multirow{2}{*}{type}    & \multicolumn{2}{c|}{Trained Data}    &\multicolumn{2}{c|}{New Data}                    \\   \cline{3-6}
 &  &{Prec.} & {Rec.} & {Prec.}  & {Rec.}              \\   \hline 
\multirow{5}{*}{5} & car& 81.8 &73.1 & 73.8   & 46.3   \\   \cline{2-6}  
 & plane & 88.3 & 80.7 & 81.1   & 72.5                 \\   \cline{2-6} 
 & camera & 98.1 & 96.4 & 95.2   &  87                 \\   \cline{2-6} 
 & cup & 42.2 & 37.5 & 31   &   22.6                   \\   \cline{2-6} 
 & landscape & 71.7 & 44.9 & 67.9   & 54.3             \\   \hline 
 \multicolumn{2}{|c|}{Average}   & 76.42 & 66.52 &69.8 & 56.54 \\ \hline 
 \end{tabular}
 \end{table}

\textit{Have at least one figure for the results section highlighting a key finding or claim.}

The results section of a course report is a critical component where you are expected to present and interpret the results. This section aims to communicate the findings in a clear and organized manner.

Use tables, graphs, and charts to present numerical data. Ensure that these visuals are labeled and properly referenced in the text. This helps readers grasp the key patterns and trends at a glance. Highlight each of your results by creating subsections. For each subsection, go into detail for your interpretation. Include figures and tables to support your results. 


% \subsection{Dissemination}

## Future Work

Start off by describing the limitations of your work and what next steps can be taken to overcome them. These limitations could be due to the data, the methods or the results. Any simplifying assumptions you made should be clearly stated, and their impact on the results should be discussed. Describe some natural next steps and extensions of your work. Talk about how such extensions and future versions of your work would be useful and what are some of the challenges that you might face in implementing them.

