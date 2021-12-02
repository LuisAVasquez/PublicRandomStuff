# TRIEs in python

TRIEs are useful for quick storage: saving, searching, and deleting.

The speed comes from the fact that the path to were a value is stored is determined by the value itself.



More info: 
https://en.wikipedia.org/wiki/Trie

In my implementation each node is a single character, and I only store strings in the TRIE.

Just follow the path determined by the characters of the string:

```
the lexicon is:  ['they', 'them', 'theirs', 'she', 'her', 'hers', 'he', 'him', 'his']
 __root__ 
> t 
>> h 
>>> e 
>>>> y Stored: they
>>>> m Stored: them
>>>> i 
>>>>> r 
>>>>>> s Stored: theirs
> s 
>> h 
>>> e Stored: she
> h 
>> e Stored: he
>>> r Stored: her
>>>> s Stored: hers
>> i 
>>> m Stored: him
>>> s Stored: his


```
