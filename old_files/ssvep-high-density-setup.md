\documentclass[]{article}
\usepackage{lmodern}
\usepackage{amssymb,amsmath}
\usepackage{ifxetex,ifluatex}
\usepackage{fixltx2e} % provides \textsubscript
\ifnum 0\ifxetex 1\fi\ifluatex 1\fi=0 % if pdftex
  \usepackage[T1]{fontenc}
  \usepackage[utf8]{inputenc}
\else % if luatex or xelatex
  \ifxetex
    \usepackage{mathspec}
    \usepackage{xltxtra,xunicode}
  \else
    \usepackage{fontspec}
  \fi
  \defaultfontfeatures{Mapping=tex-text,Scale=MatchLowercase}
  \newcommand{\euro}{€}
\fi
% use upquote if available, for straight quotes in verbatim environments
\IfFileExists{upquote.sty}{\usepackage{upquote}}{}
% use microtype if available
\IfFileExists{microtype.sty}{%
\usepackage{microtype}
\UseMicrotypeSet[protrusion]{basicmath} % disable protrusion for tt fonts
}{}
\ifxetex
  \usepackage[setpagesize=false, % page size defined by xetex
              unicode=false, % unicode breaks when used with xetex
              xetex]{hyperref}
\else
  \usepackage[unicode=true]{hyperref}
\fi
\hypersetup{breaklinks=true,
            bookmarks=true,
            pdfauthor={},
            pdftitle={},
            colorlinks=true,
            citecolor=blue,
            urlcolor=blue,
            linkcolor=magenta,
            pdfborder={0 0 0}}
\urlstyle{same}  % don't use monospace font for urls
\usepackage{graphicx,grffile}
\makeatletter
\def\maxwidth{\ifdim\Gin@nat@width>\linewidth\linewidth\else\Gin@nat@width\fi}
\def\maxheight{\ifdim\Gin@nat@height>\textheight\textheight\else\Gin@nat@height\fi}
\makeatother
% Scale images if necessary, so that they will not overflow the page
% margins by default, and it is still possible to overwrite the defaults
% using explicit options in \includegraphics[width, height, ...]{}
\setkeys{Gin}{width=\maxwidth,height=\maxheight,keepaspectratio}
\setlength{\parindent}{0pt}
\setlength{\parskip}{6pt plus 2pt minus 1pt}
\setlength{\emergencystretch}{3em}  % prevent overfull lines
\providecommand{\tightlist}{%
  \setlength{\itemsep}{0pt}\setlength{\parskip}{0pt}}
\setcounter{secnumdepth}{0}

\date{}

% Redefines (sub)paragraphs to behave more like sections
\ifx\paragraph\undefined\else
\let\oldparagraph\paragraph
\renewcommand{\paragraph}[1]{\oldparagraph{#1}\mbox{}}
\fi
\ifx\subparagraph\undefined\else
\let\oldsubparagraph\subparagraph
\renewcommand{\subparagraph}[1]{\oldsubparagraph{#1}\mbox{}}
\fi

\begin{document}

\section{Post Session Protocol High Density
EEG}\label{post-session-protocol-high-density-eeg}

\subsection{On NetStation Mac}\label{on-netstation-mac}

\begin{itemize}
\tightlist
\item
  Reminder: If you have not done so, save and close Net Station by
  pressing the \textbf{Close Session} button in the upper right hand
  corner of the NetStation window.
\end{itemize}

\subsubsection{Open Session}\label{open-session}

\begin{itemize}
\tightlist
\item
  From the Net Station startup screen, go to \textbf{File \textgreater{}
  Open} to access archived sessions.\\
\item
  Session files are usually located in:
  /Users/GilmoreLab/Documents/NetStation User Data/Sessions
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/NS_Open_Archived_Files.jpg}
\caption{NS Open Archived Files}
\end{figure}

\begin{itemize}
\tightlist
\item
  to find the most recent session, click on the \textbf{Date} field in
  the Finder window. The small arrow should face downward to sort files
  in reverse date order (most recent first)
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Finder Window arrow facing downward}
\end{figure}

\subsubsection{Run Waveform Tools}\label{run-waveform-tools}

\begin{itemize}
\tightlist
\item
  From the \textbf{Tools} menu, open \textbf{Waveform Tools}
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/NS_Open_Waveform_Tools.jpg}
\caption{NS Open Waveform Tools}
\end{figure}

\begin{itemize}
\tightlist
\item
  Run the Conatenate tool\\
\item
  Press the \textbf{Add} button, and add the session file you wish to
  the Inputs window\\
\item
  Select the \textbf{Concatenate Epochs for PowerDiva} tool from
  Specifications window

  \begin{itemize}
  \tightlist
  \item
    To monitor progress, press the \textbf{Jobs/Results} button\\
  \item
    To run the tool, press the \textbf{Run} button
  \end{itemize}
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/run-concatenate-tool.jpg}
\caption{NS Concatenate Tool}
\end{figure}

\begin{itemize}
\tightlist
\item
  Run the Export to Power Diva tool
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/NS_Export_PowerDiva.jpg}
\caption{NS Export\_PowerDiva}
\end{figure}

\begin{itemize}
\item
  Add the \textbf{.cat} file you just created to the Inputs window by
  pressing the \textbf{Add} button\\
\item
  Select the \textbf{Export for PowerDiva} tool from Specifications
  window

  \begin{itemize}
  \tightlist
  \item
    To monitor progress, press the \textbf{Jobs/Results} button\\
  \item
    To run the tool, press the \textbf{Run} button\\
  \item
    This can take 3-8 minutes.
  \end{itemize}
\item
  Quit Net Station
\item
  Quit the PowerDiva Video application on the PDvideo computer if you
  have not already done so.
\end{itemize}

\subsubsection{Transfer data for
analyses}\label{transfer-data-for-analyses}

\paragraph{Transfer to PDVideo}\label{transfer-to-pdvideo}

\begin{itemize}
\tightlist
\item
  On the NetStation computer desktop, double-click the
  \textbf{NetStation\_Sessions@PDVideo alias} (highlighted in green)
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/NS_@PDVideo.jpg}
\caption{NS Sessions @ PDvideo alias}
\end{figure}

\begin{itemize}
\tightlist
\item
  Create a new folder with the participant ID (e.g.~YYMMDDXXXX - test
  date (year, month, day) 4 digit participant ID \#\\
\item
  Double click on \textbf{Sessions@Local} (highlighted in red). This
  opens a separate window to the local NetSataion Sessions folder.
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/NS_Sessions_Local.jpg}
\caption{NS Sessions @ Local}
\end{figure}

\begin{itemize}
\tightlist
\item
  Select the files for copy to the PDVideo machine (via the green
  folder)\\
\item
  Copy the following:

  \begin{itemize}
  \tightlist
  \item
    \textbf{original session file}\\
  \item
    \textbf{raw data file} (.raw)\\
  \item
    \textbf{cat data file} (.cat)\\
  \item
    \textbf{gains file} (.GAIN)\\
  \item
    \textbf{zero file} (.ZERO)\\
  \item
    \textbf{impedance file} (.IMP)\\
  \end{itemize}
\item
  \textbf{Shift} or \textbf{command+Click} on these files and drag them
  to the green Net Station folder.

  \begin{itemize}
  \tightlist
  \item
    This can take 5-10 minutes.
  \end{itemize}
\end{itemize}

\includegraphics{imgs/NS_TransferedFiles.jpg} - Take New Picture

Take new picture of files copying.

\begin{itemize}
\tightlist
\item
  Once copied, shut own the NetStation computer
\end{itemize}

\subsection{On PowerDiva Computer}\label{on-powerdiva-computer}

\subsubsection{Duplicate Stimulus Set}\label{duplicate-stimulus-set}

\begin{itemize}
\tightlist
\item
  On the PDvideo computer make a copy (\textbf{file \textgreater{}
  duplicate}) (Command + d) of the stimulus set (found in
  \textbf{stimulus set} folder on the desktop) and put this in the
  participant's folder within the NetStations session folder.
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Copy Stimulus Set to Net Station Sessions folder}
\end{figure}

\subsubsection{Open Power Diva}\label{open-power-diva}

\begin{itemize}
\tightlist
\item
  Open the Power Diva Host 3.4 application by double clicking the icon
  on the desktop
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Power Diva Host 3.4.0 Alias Icon}
\end{figure}

\begin{itemize}
\tightlist
\item
  Ignore error messages and choose to work offline.
\end{itemize}

\subsubsection{Import NS Session}\label{import-ns-session}

\begin{itemize}
\tightlist
\item
  Import NS Session by choosing \textbf{File \textgreater{} Import NS
  Session}

  \begin{itemize}
  \tightlist
  \item
    Choose the file from the \textbf{NetStation\_sessions} folder on the
    desktop.
  \end{itemize}

  \begin{figure}[htbp]
  \centering
  \includegraphics{imgs/.jpg}
  \caption{NetStation\_sessions folder on desktop}
  \end{figure}
\item
  Session window: Enter operator and participant information\\
\item
  Operator: Complete First and Last Name\\
\item
  Participant

  \begin{itemize}
  \tightlist
  \item
    First Name = blank\\
  \item
    Last name = participant ID Code (e.g.~yymmddXXXX)\\
  \item
    Birthday and Due Date = Birthday\\
  \end{itemize}
\item
  Net Station Recording

  \begin{itemize}
  \tightlist
  \item
    Raw EEGs: Click \textbf{choose} then select the .raw file in the
    NetStation\_sessions folder you just copied the files to.
  \end{itemize}
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/PD_Choosing_Rawfile.jpg}
\caption{PD Choose Rawfile}
\end{figure}

\begin{verbatim}
- Zeros/Gains: Click **choose** then **shift-click** on both the .ZERO and .GAIN files within the participant's session folder.  
\end{verbatim}

\begin{itemize}
\tightlist
\item
  Stimuli

  \begin{itemize}
  \tightlist
  \item
    Stim Set/Ssn: Click \textbf{choose} then navigate to the duplicate
    file within the participant's session folder.
  \end{itemize}
\item
  If loaded correctly you should see valid data appear in the Video
  System, Display Type and Video Mode fields.
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{PD NS Session Info}
\end{figure}

\begin{itemize}
\tightlist
\item
  Click \textbf{OK} to import the data into Power Diva Host.
\end{itemize}

\subsubsection{Checking for Artifacts}\label{checking-for-artifacts}

\begin{itemize}
\tightlist
\item
  Power Diva will automatically check for artifacts, after which you may
  change the rejection threshold.
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/PD_Artifact_Check.jpg}
\caption{Power Diva Artifact Check}
\end{figure}

\begin{itemize}
\tightlist
\item
  Change rejection threshold

  \begin{itemize}
  \tightlist
  \item
    Adults = 50\\
  \item
    Children = 60\\
  \end{itemize}
\item
  Click \textbf{Repeat Detection}\\
\item
  Click \textbf{OK} to continue
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Power Diva Channel Substitution Parameters}
\end{figure}

\subsubsection{Analysis Parameters}\label{analysis-parameters}

\begin{itemize}
\tightlist
\item
  Set \textbf{Processing Task}-harmonics of interest for analysis
\item
  This is usually set up beforehand, but be sure to select all multiples
  of F1 (1F1, 2F1, 3F1, 4F1, 5F1, 6F1, 7F1, 8F1, 9F1). Then select 1F2,
  1F1 + 1F2, and 1F1 - 1F2
\item
  Click \textbf{Set To All} above the title `Processing Task'
\item
  Set \textbf{Epoch Rejection Parameters}
\item
  Change Raw Threshold Detector (adults 50, \textbf{children 60})
\item
  Click \textbf{Set To All} above the title `Epoch Rejection Parameters'
\item
  Click \textbf{Continue} to view the imported PD session
\item
  This takes \textasciitilde{}10 minutes to run
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Power Diva Analysis Parameters}
\end{figure}

\subsubsection{Export MATLAB data}\label{export-matlab-data}

\begin{itemize}
\tightlist
\item
  Go to \textbf{File \textgreater{} Export}\\
\item
  Export Window\\
\item
  Export as: Matlab Files
\item
  Matlab Options

  \begin{itemize}
  \tightlist
  \item
    Under \textbf{Axx Filter}, change P-thresh to \textbf{0.05}
  \end{itemize}
\item
  Data Types

  \begin{itemize}
  \tightlist
  \item
    Check the box for \textbf{Axx}
  \end{itemize}
\item
  Click \textbf{Export}
\item
  When exported, click \textbf{Done}
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Power Diva Export to Matlab files}
\end{figure}

\begin{itemize}
\tightlist
\item
  Close the session
\item
  Click the \textbf{Close} button net to the Session window
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Close Session}
\end{figure}

\subsubsection{Export RLS data}\label{export-rls-data}

\begin{itemize}
\tightlist
\item
  Go to \textbf{R\&D \textgreater{} Batch Export ODBC\ldots{}}\\
\item
  A window will open concerning bins\\
\item
  \textbf{Export No Bins}\\
\item
  sweeps = \textbf{Export Bins}
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Bins}
\end{figure}

\begin{itemize}
\tightlist
\item
  Window \textbf{Choose Source Folder}\\
\item
  Navigate to the desktop and double click on the Power Diva alias
  folder
\item
  Highlight the session of choice
\item
  Press \textbf{Choose}
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Choose Source Folder}
\end{figure}

\begin{itemize}
\tightlist
\item
  Window \textbf{Choose Export Folder}\\
\item
  Navigate to the desktop and select an external storage devic (such as
  a USB)\\
\item
  Double Click on this device\\
\item
  Press the \textbf{New Folder} button\\
\item
  Name this folder according the participant id and project name.\\
\item
  Highlight this folder and press the \textbf{Choose} button.
\end{itemize}

\begin{figure}[htbp]
\centering
\includegraphics{imgs/.jpg}
\caption{Choose Export Folder}
\end{figure}

\subsubsection{Compress and Save Files}\label{compress-and-save-files}

\begin{itemize}
\item
  Duplicate the files below and compress them using \textbf{Dropstuff}\\
\item
  .pdh file\\
\item
  Data\_mtg0\\
\item
  Data\\
\item
  Exp\_MATL\_HCN\_128\_Avg\\
\item
  \emph{Stimulus\_Set\_}Copy
\item
  Add the files below to the Participant's folder on the external
  drive:\\
\item
  .pdh file.sit\\
\item
  Data\_mtg0.sit\\
\item
  Data.sit\\
\item
  Exp\_MATL\_HCN\_128\_Avg.sit\\
\item
  \emph{Stimulus\_Set\_}Copy.sit\\
\item
  \textbf{original Net Station session file}\\
\item
  \textbf{Net Station raw data file} (.raw)\\
\item
  \textbf{Net Station cat data file} (.cat)\\
\item
  \textbf{Net Station gains file} (.GAIN)\\
\item
  \textbf{Net Station zero file} (.ZERO)\\
\item
  \textbf{Net Station impedance file} (.IMP)
\item
  RLS.txt file\\
\item
  CndParams file\\
\item
  QETXT file\\
\item
  SCHEMA.INI file\\
\item
  SSNHeader.txt file
\item
  Remove storage device and load onto computer with Matlab for analysis
  (separate protocol)
\end{itemize}

\end{document}
