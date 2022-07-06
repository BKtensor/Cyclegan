# tensorflow
BK's models

I will restore my models here

Cyclegan is a  model to do 'sytle transfer'.
It contains 2 generators and 2 discriminators

Genrator X : to generater a man's photo,based on a woman's photo(condition).
Genrator Y : to generater a woman's photo,based on a man's photo(condition).
discriminators X : to judge the man's photo, is it a fake one or real one?
discriminators y : to judge the woman's photo, is it a fake one or real one?

Here's the training method:
1.real man-> gen x -> fake woman -> dis y --> real or fake?
                                 -> gen y -> fake man' --> loss with real man?

2.real woman->gen y -> fake man -> dis x --> real or fake?
                                -> gen x -> fake woman' --> loss with real woman?
                                
                                
