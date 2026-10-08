# Unit - 4
# Cascading Style Sheet

## syntax 

            selector
            {
                property : value;
                property : value;
            }                    

## Types of CSS :

1. inline CSS

        <p style = "color:red ;"> Hello </p>

2. Internal CSS

        <head>
            <Style>
                p
                {
                    color:red;
                    background-color:green;
                }
            </Style>
        </head>

3. External CSS

*p1.css*

        p
        {
            color:red;
        }

*p1.html*   

        <head>
            <link rel="stylesheet" href="p1.css"/>
        </head>

----------------------------
----------------------------

> if the properties are same then ,
**priority : inline CSS > inline CSS > external CSS**   
--------------
## Text Properties
1. color
2. text-align       - left , right , center , justify
3. text-indent      - % , px
4. text-transform   - none , capitalize , uppercase , lowercase
5. text-decorartion - none , overline , underline , line-through , underline overline
6. letter-spacing   - px
7. word-spacing     - px
8. line-height      - number , px , %
9. text-shadow      - h-shadow v-shadow blur color 2px 2 px 4px red

--------------
## Font Properties
1. font-family
2. font-size - (px,%) *or* xx-small,x-small,small,large,x-large,xx-large)
3. font-style - normal,italic
4. font-weight - bold (100...900)
5. font-variant - normal , small-caps

------
## Border Properties
1. border-style - none,solid,dashed,dotted,double
2. border-width - px
3. border-color
4. border-radius - px , %  *(div height : 200 width : 200 border-radius:50% :: gives circle)*

### shorthand
1. border : width(opt) style(Must) color(opt)

*e.g. border : 2px double green*

*can write border-left or border-right as well*


## CSS selectors

| Type    | Syntax | Ex |
| -------- | ------- | --- |
| Element  | element    | p{color:black} |
| ID | #id     | #id{color:blue} |
| Class    | .class    | .class{color:green} |
| Attribute  | [after=value] | [type="text"] { color : blue } |
| Universal | * | * {color:red } |
| Descendant | ancestor descendant | div p { color:red } |
| Child | Parent>child | div>p {color : blue }
| Grouping | selector1 , selector 2 | h1 , h2 , h3 { font-size : 20px } |

------
> **only 1 id is allowed to use in 1 tag <p id="[value]">**
**but multiple classes <p class="[class1] <space> [class2]">**