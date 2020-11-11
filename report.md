---
# Please do not delete --- above :) 

# ========================================================================
# Automatically edited by GitHub actions, please do not modify     | START 
# ==============================================================
report_url: https://github.com/brainhack-proceedings/template

last_changed: 2020-11-11 03:39 UTC

auth_created: agahkarakuzu
# ===============================================================  | END 

# Name of the event. 
# -----------------
event: 'OHBM Brainhack 2020'

# The title of your report. 
# -------------------------
title:  'An automagical report generator for BrainHack Proceedings'

# Please SET this url to your GitHub project repo!
# ------------------------------------------------- 
url: https://github.com/username/project_repository 

# Please edit affiliation details. The affiliation 
# ids defined here will be used in the author list.
# ------------------------------------------------- 
affiliations:
- id: aff1
  orgname: 'Research Lab 1, Organization 1'
  street: street_name_goes_here 
  postcode: post_code_goes_here
  city: Montreal
  state: Quebec
  country: Canada
- id: aff2
  orgname: 'Research Lab 2, Organization 2'
  street: street_name_goes_here 
  postcode: post_code_goes_here
  city: Montreal
  state: Quebec
  country: Canada

# Please list the authors.
# If an author has multiple affiliations, please
# add corref field and indicate the primary affiliation.
# -----------------------------------------------------
author:
- initials: JD
  surname: Doe
  firstname: Jane
  email: janedoe@gmail.com
  affiliation: aff1, aff2
  corref: aff1
  # Please make sure that you set corref (corresponding aff) if you have
  # multiple afiliations
- initials: JJD
  surname: Doe
  firstname: John J.
  email: johndoe@gmail.com
  affiliation: aff2
  url: https://jonhdoe.website.com

# Please write a brief summary of your project.
# This abstract will (only) appear on the webpage.
# -------------------------------------------------
summary: Powered by GitHub Actions, Pandoc and Hugo, this simple repository can turn itself into a full-blown article page where you can download the PDF! Zero installation. We hope that this little project encourages all the great hackathon participants to create nifty reports worthy of their projects. If you have any suggestions or improvements, please feel free to open an issue or make a pull request at the brainhack-proceegins/template repository.

# Please add 1 to 3 tags
tags:
  - tag1
  - tag2
  - tag3

# Please comment out the following 5 lines if you have no supplemental material.
supplemental:
  - name: Material 1
    url: https://osf.io 
  - name: Material 2 
    url: https://zenodo.org 

coi: Please add if there are competing interests. Otherwise, type None.

acknow: The authors would like to thank the organizers and attendees of OHBM Brainhack 2020.

contrib: JD and JJD wrote the software, JD performed tests, and JD and JJD wrote the report.

# Please comment out the following 4 lines if no reviewer has been assigned to you yet.
reviewers:
  - name: Agah
    surname: Karakuzu
    gh_handle: agahkarakuzu

# Show/hide the BinderHub (mybinder.org) badge
# Accepted values: true/false (case sensitive)
# -------------------------------------------
binder: true

# Enable/disable hypothes.is
# Accepted values: true/false (case sensitive)
hypothesis: true

# Please do not delete --- below :) 
---

# Introduction
The bibliography \code{report.bib} must respect \href{http://www.bibtex.org/Using/}{BibTeX} format. 
You can cite entries in your bibliography using their tags:

\begin{itemize}
  \item Cite an article: \cite{author:2010}
  \item Cite a GitHub repository: \cite{githubrepo:2020}
\end{itemize}

\smallskip
\noindent You can use \code{inline code highlight}. This paragraph shows how to add blank lines and how to start a paragraph without indentation.

Remember that this is a LaTex flavored markdown. Therefore, some characters must be used with an escape character within the text:

\code{\& \% \$ \# \_ \{  \} \textbackslash}


# Section
You can create additional sections as you prefer. Section title levels are determined by the number of hastags as in a traditional markdown file.

## Subsection
Subsection content goes here. You can create numerated lists:

\begin{enumerate}
  \item The labels consists of sequential numbers.
  \item The numbers starts at 1 with every call to the enumerate environment.
\end{enumerate}

### Equations & formulas
You can add mathematical formulas. Single dollars ($) are required for inline mathematics e.g. $f(x) = e^{\pi/x}$.
\smallskip

\noindent You can also use plain LaTeX for equations. These equations are rendered by MathJax, you can right click on them and explore the rendering options available at your browser!

\begin{equation} \label{eq:1}
\hat f(\omega) = \int_{-\infty}^{\infty} f(x) e^{i\omega x} dx
\end{equation}

and refer to \ref{eq:1} from text.

### Hypothes.is 
We enabled \href{https://web.hypothes.is/}{hypothes.is} for the brainhack proceeding reports. This way, you can annotate, highlight and tag the content collaboratively! You may choose to share your insights with everyone, or keep them private.      

# Results
Figure files must be placed at the \code{figures} folder. You can include figures using the following block:

\begin{figure}[h!]

  \includegraphics[width=.47\textwidth]{brainhack.png}

  \caption{\label{Figure-1} Your caption goes here.}

\end{figure}

Note that \code{width=.47 \textbackslash textwidth} above sets scales the figure size in the PDF. To change attributes of the figures on the webpage, please see \code{/figures/figures.css}. 

To refer a figure in the text, you need to use the respective label defined in its caption: Fig. \ref{Figure-1}
