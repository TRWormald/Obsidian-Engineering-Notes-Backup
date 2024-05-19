```tikz
\begin{document}
\usepackage{pgf-plots}
\tikzset{
pattern size/.store in=\mcSize, 
pattern size = 5pt,
pattern thickness/.store in=\mcThickness, 
pattern thickness = 0.3pt,
pattern radius/.store in=\mcRadius, 
pattern radius = 1pt}
\makeatletter
\pgfutil@ifundefined{pgf@pattern@name@_f49qvroyt}{
\pgfdeclarepatternformonly[\mcThickness,\mcSize]{_f49qvroyt}
{\pgfqpoint{0pt}{0pt}}
{\pgfpoint{\mcSize}{\mcSize}}
{\pgfpoint{\mcSize}{\mcSize}}
{
\pgfsetcolor{\tikz@pattern@color}
\pgfsetlinewidth{\mcThickness}
\pgfpathmoveto{\pgfqpoint{0pt}{\mcSize}}
\pgfpathlineto{\pgfpoint{\mcSize+\mcThickness}{-\mcThickness}}
\pgfpathmoveto{\pgfqpoint{0pt}{0pt}}
\pgfpathlineto{\pgfpoint{\mcSize+\mcThickness}{\mcSize+\mcThickness}}
\pgfusepath{stroke}
}}
\makeatother
\tikzset{every picture/.style={line width=0.75pt}} %set default line width to 0.75pt        

\begin{tikzpicture}[x=0.75pt,y=0.75pt,yscale=-1,xscale=1]
%uncomment if require: \path (0,300); %set diagram left start at 0, and has height of 300

%Shape: Rectangle [id:dp31934278564593965] 
\draw  [pattern=_f49qvroyt,pattern size=11.25pt,pattern thickness=0.75pt,pattern radius=0pt, pattern color={rgb, 255:red, 0; green, 0; blue, 0}] (100,85) -- (171.67,85) -- (171.67,259) -- (100,259) -- cycle ;
%Straight Lines [id:da6603429863635861] 
\draw    (171.67,259) -- (480.67,259) ;
%Straight Lines [id:da8178077344318859] 
\draw [draw opacity=0]   (171.67,85) -- (480.67,85) ;
%Straight Lines [id:da893150673530023] 
\draw [draw opacity=0][fill={rgb, 255:red, 74; green, 144; blue, 226 }  ,fill opacity=1 ]   (480.67,85) -- (480.67,259) ;
%Shape: Rectangle [id:dp9176660324505734] 
\draw  [draw opacity=0][fill={rgb, 255:red, 74; green, 144; blue, 226 }  ,fill opacity=0.26 ] (171.67,85) -- (480.67,85) -- (480.67,259) -- (171.67,259) -- cycle ;
%Straight Lines [id:da8884399717647049] 
\draw    (289.83,249.83) -- (174.5,249.83) ;
\draw [shift={(172.5,249.83)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da9397951667808688] 
\draw    (280.83,230.08) -- (173.5,230.08) ;
\draw [shift={(171.5,230.08)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da05820952382520583] 
\draw    (270.08,209.83) -- (173.75,209.83) ;
\draw [shift={(171.75,209.83)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da46326694645549793] 
\draw    (260.33,190.83) -- (174.25,190.83) ;
\draw [shift={(172.25,190.83)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da27377371779569804] 
\draw    (250.33,170.08) -- (174.25,170.08) ;
\draw [shift={(172.25,170.08)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da051556807623817535] 
\draw    (240.08,149.83) -- (173.25,149.83) ;
\draw [shift={(171.25,149.83)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da9329846792393697] 
\draw    (229.58,130.33) -- (174.25,130.33) ;
\draw [shift={(172.25,130.33)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da17156265535473247] 
\draw    (220.58,110.58) -- (174.75,110.58) ;
\draw [shift={(172.75,110.58)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da3374363322919809] 
\draw    (209.83,90.08) -- (173.75,90.08) ;
\draw [shift={(171.75,90.08)}, rotate = 360] [color={rgb, 255:red, 0; green, 0; blue, 0 }  ][line width=0.75]    (10.93,-3.29) .. controls (6.95,-1.4) and (3.31,-0.3) .. (0,0) .. controls (3.31,0.3) and (6.95,1.4) .. (10.93,3.29)   ;
%Straight Lines [id:da8663394962898612] 
\draw [color={rgb, 255:red, 208; green, 2; blue, 27 }  ,draw opacity=1 ][line width=3]    (280.5,170.17) -- (177.25,170.09) ;
\draw [shift={(172.25,170.08)}, rotate = 0.04] [color={rgb, 255:red, 208; green, 2; blue, 27 }  ,draw opacity=1 ][line width=3]    (20.77,-6.25) .. controls (13.2,-2.65) and (6.28,-0.57) .. (0,0) .. controls (6.28,0.57) and (13.2,2.66) .. (20.77,6.25)   ;
%Straight Lines [id:da3040344433232258] 
\draw [color={rgb, 255:red, 208; green, 2; blue, 27 }  ,draw opacity=1 ][line width=3]    (306,201.17) -- (177.25,200.61) ;
\draw [shift={(172.25,200.58)}, rotate = 0.25] [color={rgb, 255:red, 208; green, 2; blue, 27 }  ,draw opacity=1 ][line width=3]    (20.77,-6.25) .. controls (13.2,-2.65) and (6.28,-0.57) .. (0,0) .. controls (6.28,0.57) and (13.2,2.66) .. (20.77,6.25)   ;

% Text Node
\draw (285,161) node [anchor=north west][inner sep=0.75pt]   [align=left] {{\scriptsize Force through the centroid}};
% Text Node
\draw (307,191.5) node [anchor=north west][inner sep=0.75pt]   [align=left] {{\scriptsize Force through the centre of pressure}};


\end{tikzpicture}
\end{document}
```
