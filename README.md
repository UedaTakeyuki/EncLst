# Enclst
## What is it?
The enclst is a notation rule for **humans** to write a list structure **concisely**.

## What is it for?
This is for what humans write a **list of data** with **attributes** and **title string** that a computer handles the data. Typically the data is something ID like a **URL of a website** or a **content ID of YouTube**. 

## Why not JSON?
JSON is a rich notation enough to represent general objects including lists. There is no difficulty for a computer program to handle a JSON. However it comes to humans, it isn't easy to write a no-error JSON string. When you try to write JSON by hand, you may notice the following pitfalls:

- Prohibition of dangling commas
- String escaping

Even experienced software engineers (like me :-) write a JSON by hand carefully, it's impossible to continue writing without any errors. Furthermore, asking **non-engineering end users** to input **error-free JSON** is unreasonable.

This is exactly my motivation for creating enclst. JSON is impossible for a non-engineer end user. A more succinct alternative must be necessary.

# Enclst Notation
An **Enclst** is a multi-line string separated by line breaks. The **first line** is the **Title** of the Enclst, followed by the **ItemList** separated by **a blank line** illustrated as follow:

![](draw.io/overallView/overallview.jpg)

The **ItemList** is a multi-line string that is the remainder of Enclst followed by The **Title** and a blank separator line, and each low is one **Item**. An Item is consist of **Value** and **Title** separated by a vertical line "**|**".

![](draw.io/Item/Item.jpg)

A value can have several values separated by comma "**,**".

Note: In a title string, any escaping is not needed. Even commas "**,**" and vertical lines "**|**", you can use them **without escaping**.
```
https://www.bhg.com/gardening/plant-dictionary/ | Titles like this, |also| OK!
```

More detail of Enclst Notation is available [here](documents/Enclst.md).

# Application examples

## For Website URL
[EncycloList](https://encyclolist.uedasoft.com/): A browser to display the list of Items consists of a **website URL** and a **its title**, and opens the URL in which selected Item.
- [British Newspapers](https://encyclolist.uedasoft.com/list/https:%2F%2Fraw.githubusercontent.com%2FUedaTakeyuki%2FEncLst%2Fmain%2Fexamples%2FEncycloList%2Flang%2Fen%2Fnewspaper%2Fnewspaper.enclst): displaying enclst is [here](https://github.com/UedaTakeyuki/EncLst/blob/main/examples/EncycloList/lang/en/newspaper/newspaper.enclst)
- [Journal Française](https://encyclolist.uedasoft.com/list/https:%2F%2Fraw.githubusercontent.com%2FUedaTakeyuki%2FEncLst%2Fmain%2Fexamples%2FEncycloList%2Flang%2Ffr%2Fjournal%2Fjournal.enclst): displaying enclst is [here](https://github.com/UedaTakeyuki/EncLst/blob/main/examples/EncycloList/lang/fr/journal/journal.enclst)
  - [more examples…](https://github.com/UedaTakeyuki/EncLst/wiki/EncycloList-example-pages)
 
## For Youtube Contents
- [HS](https://hs.uedasoft.com/channel2/home): A brouser to display the list of Items consists of a **youtube contents ID** and **its title**, and play the contents in which selected Item.
