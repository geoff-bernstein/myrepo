....

---
title: "RMD Template"
author: "sulgrave"
date:  
output: md_document <!--word_ pdf_ or html_document
                      beamer_, ioslides, or
                      slidy_presentation-->
---

# Header 1 {#anchor}

```{r}
Post an r code block
'''{r, with the following arguments}

results = 'hide'      runs code in background           no display
echo = FALSE          hides only code itself            evaluates code and displays output 
eval = FALSE          displays only code itstelf        no evaluation and no output
engine = 'python'     displays as pythoncode
```
inline r code is sexy: `r factorial(4)` 

<br><br><br>
      
## Header 2: Some LaTeX Examples {#css_id}
$$ ozone = \alpha + \beta_{1} temperature + \sum_{locales} \beta_{i} locale_{i} + \sum_{locales} \beta_{j} interaction_{j} + \epsilon$$

$$ \min_{\beta_0,\beta} \frac{1}{N} \sum_{i=1}^{N} w_i l(y_i,\beta_0+\beta^T x_i) + \lambda\left[(1-\alpha)||\beta||_2^2/2 + \alpha ||\beta||_1\right]$$


> 
The elastic-net penalty is controlled by $\alpha$, and bridges the gap between lasso $\alpha = 1$, the default and ridge, $\alpha = 0$. 
> The tuning parameter $\lambda$ controls the overall strength of the penalty.
  
  <br><br><br>
  
### Header 3: Displaying and Modifying Text {.css_class}
W/ Plain text, End a line with two spaces to start a new paragraph.  
*italics* and **bold**  
Emphasized text <em>italicizes and jumps out</em> 
`verbatim code in monospace text`  
sub~2~ / superscript^2^
~~strikethrough~~  
escaped characters: \* \_ \\  
endash: --, emdash: ---  
in-line equation: $A = \pi*r^{2}$  
equation block: $$E = mc^{2}$$  
<!--Text comment not printed to output-->
\textbf{Tex ignored in HTML}  
URLs with <http://www.rstudio.com> or [link](www.rstudio.com)  
Jump to [Header 1](#anchor)  
Jump to [Header 4](#anchor)

#### Header 4
##### Header 5
###### Header 6


image:
![Caption] (smallorb.png)

* unordered list
 + sub-item 1
 + sub-item 2
 - sub-sub-item 1

* item 2
 Continued (indent 4 spaces)

* **bullet** -  using asterisk
- **bullet** -  using a single dash

1. ordered list
2. item 2
      i) sub-item 
      A. sub-sub-item 
* apple
* pear 
* banana

- apple
- pear
- banana

Or ordered lists:

1. items
1. are
1. automatically
1. ordered
    - nested
        * items
        
(@) An Ordered List  
(@) whose numbering  
continues after  
(@) an interruption 
    i) and can still have  
      A. sub items  
<br>
 
>- to have bullets appear on click  
horizontal rule/slide break:  
<br>
***

Bibliography Citations:
Smith cited [@smith04].
Smith cited without author [-@smith04].
@smith04 cited in line.

A footnote [^1]  
[^1]: Here is the footnote
 
 
