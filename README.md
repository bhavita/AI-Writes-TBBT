# AI Writes TBBT
Taking help of GPT-2 model and training it for The Big Bang Theory corpus, let AI write TBBT for us <3 

## Inspiration 
My close friends and I have been big fan of [The Big Bang Theory](https://en.wikipedia.org/wiki/The_Big_Bang_Theory). And if you are a fan, you know how much you miss the series. Insipiration was to train a model on the TBBT corpus and let AI take the essence of our beloved characters, cast its magic and write the TBBT for us which is missed.

## DataSets utilized for training
Reference website : [bigbangtrans.wordpress.com](https://bigbangtrans.wordpress.com)

This proved to be a great reference to retrieve transcript for The Big Bang Theory Episodes. 

Example Episodes 

[https://bigbangtrans.wordpress.com/series-1-episode-1-pilot-episode/](https://bigbangtrans.wordpress.com/series-1-episode-1-pilot-episode/)

[https://bigbangtrans.wordpress.com/series-1-episode-2-the-big-bran-hypothesis/](https://bigbangtrans.wordpress.com/series-1-episode-2-the-big-bran-hypothesis/)

Steps undertaken for preparation 

1. Prepared a reference json for identifying the episodes list(as above),
2. Scraped the webpage for content containing the transcripts of episode, 
3. Cleaned up majority of surrounding tags and formatting, and the 202 episodes dataset was prepared.

DataSet - [https://github.com/bhavita/AI-Writes-TBBT/tree/master/DataSet](https://github.com/bhavita/AI-Writes-TBBT/tree/master/DataSet)
   
   This dataset was then used to train the model.



## Implementation

Model trained over GPT-2 - 
Implementation : - [AI-Writes_TBBT.ipynb](https://github.com/bhavita/AI-Writes-TBBT/blob/master/AI_Writes_TBBT_Using_GPT_2_Text_Generating_Model.ipynb)

Minor details regarding parameterization 

| Parameter |Data  |
|-|--|
| DataSet Size|3254056 characters|
| Pretrained Model Used |124M  |
| Steps |1000  |
| _Top-p_ sampling |0.9  |
| Temperature |0.8  |
| Samples generated |20  |
| Batches |20  |
| Length of target |100 characters  |





## Sample generation Text From The Trained Model

While honestly 50% texts generated din make relevant sense, it was pretty funny to see them turn out :) 

**Starting scene provided to the model:** 

    Scene: The comic book store.
    Leonard: Who would win in Batman vs Superman fight?
 
 **Generated Texts**

 *Sample Text 1*

    Scene: The comic book store.
    Leonard: Who would win in Batman vs Superman fight? Superman, Waluigi, Wonder Twins, Dr. Jekyll
    and Mrs. Whore?
    Sheldon: I’m sorry, Dr. Whore? I was thinking of putting a damper on the whole DC multiverse, 
    not just the one where Superman is king.
    Leonard: Great, I’m going to start a new one.
    Sheldon: Oh, I think I saved that one for last. It’s called Jekyll and Mr Hyde.

*Sample Text 2* 

    Scene: The comic book store. 
    Leonard: Who would win in Batman vs Superman fight?
    Sheldon: I don’t know. How could Batman win? Superman has a body that looks like that of a Bat, 
    but he’s too big for Superman’s body. Batman has Superman’s Kryptonian DNA. 
    Leonard: So both? 
    Sheldon: The Dark Knight. Superman’s the son of Krypton, and Batman is his Kryptonian cousin, 
    who wants to go into space.

*Sample Text 3*
    
    Scene: The comic book store. 
    Leonard: Who would win in Batman vs Superman fight? Superman’s got that big, fiery G-string. 
    Sheldon: I’m not going to comment on the merits of a candidate, but I believe I can come up 
    with a hypothetical response. 
    Leonard: Batman might be the best superhero, but Batman doesn’t have a head. 
    Sheldon: I’m not gonna say that. I’m not gonna say it.Flash in a air.

*Sample Text 4*

    Scene: The comic book store.
    Leonard: Who would win in Batman vs Superman fight?
    Raj: I don’t know. Maybe he’ll use his superpowers to defeat Superman.
    Howard: Maybe hell use his powers to defeat the Flash.
    Raj: Maybe he'll defeat Superman by flying away from his plant in the middle of the desert sun.
    Sheldon: Superpowers? That’s funny.

## License
 
The MIT License (MIT)
Copyright (c) 2020 Bhavita Lalwani 

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
