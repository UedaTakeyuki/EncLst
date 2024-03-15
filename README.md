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

The **Enclst Notation** consists of **Title** string and **ItemList** separated by a **blank line**, fx:

```
Plant Encyclopedias

https://www.bhg.com/gardening/plant-dictionary/ | Plant Encyclopedia
https://www.plantsnap.com/plant-encyclopedia/ | Plant Encyclopedia: Complete Online Plant and Flower ...
https://www.picturethisai.com/wiki | Online Plant Encyclopedia and Common Popular Plants
```

<img src="https://viewer.diagrams.net/?tags=%7B%7D&highlight=0000ff&edit=_blank&layers=1&nav=1#R5VhLc9s2EP41nGkO1FCgnkdRkWtP09apE2dy6kAkRMIGARqERCm%2FvgsClAhRdJypnUsuIrC72P2wLwDywmW%2B%2F13iIvtTJIR5KEj2XvjeQ2g%2BncCvJhwMYTyZG0IqaWJIwxPhjn4jlhhY6pYmpHQElRBM0cIlxoJzEiuHhqUUlSu2Ecy1WuCUdAh3MWZd6heaqMxFp8nXhKaZcuk5biQtocxwIqoWKVx54VIKocwo3y8J045rnGLWXfVwj6gk4epFC%2B4fr%2FlqjUkUPYyeNovl9dMH32rZYba1u%2FXQhIG%2BKKE7DVodrBsmT1uNNNoIrvyyDtICBIbTAuIcnfgwSvX3lmHAhYIVjw8xEwVJKC49tNTRy2ipgZX1mOhfqpj%2Bis2JDQtZqRo4sK8akVH%2BWiAbPWv5KmreBmSmlM70hQ4tuqqqarDO0kEscpilWCaEU57CuNAe9xMaKyo4lodaPvCm2uWXovGzUdf4So4Li93gJQ6i7yCuTS5FXjCidL78zRnlpCWNeQK%2FV0xURId0MBj89F2C%2F7eS6CTG1O60oo%2F0uLEOZjcmdguwyVxwLSWKLcOykS%2F79oOcfSBF9ppeKikeyVIwIYHOBRgOI8xoymHKyKbeK2XsTCJTOYPZEIY7IhWFZriwi3KaJNpIVGVUkbsCx9piBZ0faFJseUJ0wwmsE207H06PILVCsu9tYsNja4TzhIicKJ3JgV0wsc3UHiX%2B1M6rU2OeNTJZuyvPLBHbwyA9qj61TBjYrvkDHXRyoYOexcIEoTk7kOtfOBYKLZfvU316DjaQu3GGpRpgzoXCupj%2FRd2oMbwm7FaUVAsAWZrNRoWgXBG52hGdLMbGKzh%2B5Dp%2B2PX7cNx1%2B%2BStvD7vPbd00r2opOc9JX2jSN6uMqPw%2BTJrxbMJU0x0GJ4rIEkADV7XqoImcrWjxpE3fq91bZUobQH1FfOF6n2FcPuhG2%2FUjff0QpmN3ireTb79YmV2DMN36gy9md%2F7L4j%2Fu9A%2BmUvfL15oaOxGfNSN%2BKUD7e0qDfVGvJDkYsC3nMbw6PPXNKEm5rQUDCvjokBfd%2FwGu%2BaGE5sRwRrHj2l9afBj41rNl%2Bn6NzSamccCGs3tYBy8s6sEXHqt7DES4PMk0RfhmozAAgqCwXBE8tO0MVsc67k2RwAr3Vk1OZYp5b4SheH6qFllOWuhFNzqzph1jpFzTHUpbHBO2cE6hmdEUpPhgYDM0X3IsDJIV8INxwa%2F3sn0CFvXgG9uWppj71wtRS3mWhL86FfgKSNy5t4QGaeGof1O3rUQt4p31CneIKHSCT9T0uVjhf0dSRwhhLPPf6yqh81482mS3uLVYv%2BFFPdfo%2Bv7vx4WT6OPIak%2BkPTjTfTP4rOjjrqKVOUrCARRft0SOobhVRGTDN74xEXpraZedOVFMJh5i5kXhc7amOGyPDdUKzRmAm1X%2B59p43aO%2B5%2BCZYH5i7rjBQfDPT911kBaPI%2F1K7r5eBX3o3lxr%2B6iMYoWejMkL9TBFrTWRqDNQeXox%2BfxBW9eL%2FAyyBl1Xu9udz%2BSjZ865LrV9BwFzVEOrZ6Jrep5irROigJKDppjnRB20e2J1HkOtV4tI5ivcanHKHydho%2FmZ0f8vNvww%2BDCGT8b%2F3DHh%2Bnp%2F6Wa1%2FqHLlz9Bw%3D%3D">

The ``first line`` is the **Title** of this Enclist which is separated from the remaining **ItemList** by a **blank line** at ``second line``.

Each part is defined as follows:

- Title  
A **single line string** that is terminated by a new line code like ``the first line``.  


- Blank line  
A blank line like ``line 2`` which has only line feed. The Encyclolist application recognizes the lines after this blank line as **itemlist.**

- ItemList  
Multiple strings where one line represents one item.

## Title

The **Title** is a **single line string** that is terminated by a new line code.  

If there are multiple lines before the first blank line, only the first line will be recognized as the title. 

```
Plant Encyclopedias, this is the title of this Enclst
This line is not title, just be ignored
This lie is also not title

https://www.bhg.com/gardening/plant-dictionary/ | Plant Encyclopedia
https://www.plantsnap.com/plant-encyclopedia/ | Plant Encyclopedia: Complete Online Plant and Flower ...
https://www.picturethisai.com/wiki | Online Plant Encyclopedia and Common Popular Plants
```

Note that the current version of the Encyclolist application simply ignores the rest of the lines, but future versions may interpret those lines to have some special meaning. Anyway, currently only the ``first line`` is recognized as the **title**

## Item List
The item list is lines of items each line consists of the **URL**, a vertical bar **|** and **item title** as follows:

```
https://www.bhg.com/gardening/plant-dictionary/ | Plant Encyclopedia
```

The Encyclolist application use the above **URL** as a bookmark link and **item title** as a line title.

More precisely, the Encyclolist application recognizes the first vertical bar delimited forward as the **URL** and the rest as the **item title**. So even if the item title string itself contains **|** , they are treated as part of the title normally.

```
https://www.bhg.com/gardening/plant-dictionary/ | ItemTitle |no problem|
```

FYI **|** is not a character that can be used in URLs so there is no real case where it appears in URLs. But in case you put **|** inside your URL, The Encyclolist application miss-recognizes the first half of the string separated by **|** as the URL.

The Encyclolist application simply discards lines that cannot be recognized as item. More precisely if there is no **|**, this line just be ignored.

## Special case

### Blank first line
In case the **first line is blank**, the Encyclolist application recognizes that this enclst has **blank title** whcih consist of only brank character. If you want to omit the title, start with a blank line like this.

```

https://www.bhg.com/gardening/plant-dictionary/ | Plant Encyclopedia
https://www.plantsnap.com/plant-encyclopedia/ | Plant Encyclopedia: Complete Online Plant and Flower ...
https://www.picturethisai.com/wiki | Online Plant Encyclopedia and Common Popular Plants
```

### Last line blank
Blank lines at the end of sentences are ignored.
```
https://www.bhg.com/gardening/plant-dictionary/ | Plant Encyclopedia
https://www.plantsnap.com/plant-encyclopedia/ | Plant Encyclopedia: Complete Online Plant and Flower ...
https://www.picturethisai.com/wiki | Online Plant Encyclopedia and Common Popular Plants



```


### No blank line
In case there are **no blank lines**, the expected Encyclolist application behaviour is **undefined**. 

The application strives to guess if the first line is the title line or the first line of Item list. It's reasonable to hope that future versions of the application will be smart enough.　But the earlier version of the application might recognize that the first line is the **title** and this ecnlst has **blank ItemList** which has no item. This is probably not the result you wanted, you simply forgot to start with a blank line to omit the title.

### Several blank lines
In case there are **several blank lines**, The Encyclolist application recognizes as **title** of the first line and as **ItemList** as remaining. Also, the Encyclolist application simply discards lines that cannot be recognized as item. As result, these multi-blank line enclst is recognized as the same as normal single blank line enclst

```
Plant Encyclopedias

https://www.bhg.com/gardening/plant-dictionary/ | Plant Encyclopedia

https://www.plantsnap.com/plant-encyclopedia/ | Plant Encyclopedia:
```

# Application examples

- [EncycloList](https://encyclolist.uedasoft.com/): A web application to read a website from enclst of **website URL**.
- [HS](https://hs.uedasoft.com/channel2/home): A web application to watch a contents from enclst of **youtube contents**.
