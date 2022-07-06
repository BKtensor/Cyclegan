# tensorflow
BK's models

I will restore my models here

Cyclegan is a  model to do 'sytle transfer'.
It contains 2 generators and 2 discriminators

Genrator X : to generater a A's photo,based on a B's photo(condition)<br/>
Genrator Y : to generater a B's photo,based on a A's photo(condition)<br/>
discriminators X : to judge the A's photo, is it a fake one or real one?<br/>
discriminators y : to judge the B's photo, is it a fake one or real one?<br/>

Here's the training method:<br/>
1.real A-> gen x -> fake B -> dis y --> real or fake?<br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;-> gen y -> fake A' --> loss with real A?<br/>

2.real B->gen y -> fake A -> dis x --> real or fake?<br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;-> gen x -> fake B' --> loss with real B?<br/>
                                
                                
