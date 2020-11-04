# Think responsivly:
## So that one makes a responsive web page, one must have a good understanding of css basic unites.
***
* * ### css unites:
* % :

      The pourcentage is a basic yet powerful css unite. It allows you to make the sizes of all components responsive by giving them a certain size compared to their father component. For example if we give a 50% width value to an <img> inside of <section/> this means that we will display an image with a width that matches 50% of the section's width.
      Here is a tip:
      -The first problem that you may face is that we must have a parent container that has a certain size. Hence, we set the background by doing this:
      html {
            height: 100%;
            }
      Moreover, we often use the min/max-width/height properties to define a min/max values to components that would take when it shrinks or grows up.
* em :

      In this section we gonna work on font-sizes. Thus, we will use the em unit. It looks for the first parent that has a certain font size value and work as percentage on ten. The default value that it takes is 16px. Consider this example:
      html {
            font-size: 16px;
            }
      section {
                font-size: 0.6em;
                }
      Remark that the problem with the em unit is that it can causes a bad cascading effect, i.e. the values of all parents affects the child. So we come up with the following solution(the next solution).
* rem :

      In fact rem means root em. Wich means that it is related to the root element, i.e. the html class element. Hence we use often absolute values or rem unite and with cauting we use less the em unite.
* vh / vw / vmin /vmax:

      Those are relative unites based on the layout height / width / min or max of those two of the view port. 
* fr :

      This is a special unite that works for grid display. It representes the size of a cell in a normal division. It is also a useful responsive unit.
* * ### how to use them:
CSS unites are generaly used like this:
em for margin and padding, rem for font size, em or percentage for width and height and we can use px to any one of them.
Remember that those aren't absolute rules they are based understanding of how those unites works.
       
    %:based on the parent element.
    px:the minimum unite independant of the screen.
    em:based on all the parent elements with font size and to the font size of the same element  e.g. 
    .parent {   
        font-size: 18px; 
        }
    .child {   
        font-size: 1.5em; 
        padding: 2em 1em;
        } .
    rem:based on the root (html) element.
***
## Types of display are also an important part of css. They decide how elements should be positioned.
***
### Types of display :
Generaly, there are three types of display inline, block and flex. They are used into parent element toghether to define how children should set.
### Media queries :
Media queries are a specific style properties that allows it to match a specific devices. It works like this :

      @media media-type and (media-featuers) {...}
      Type can be screen, print or speech.
      Features can be widht, orientation, hover ...