# tensorflow
BK's models

I will restore my models here

Cyclegan is a  model to do 'sytle transfer'.
It contains 2 generators and 2 discriminators

Genrator X : to generater a MAN's photo,based on a WOMAN's photo(condition)<br/>
Genrator Y : to generater a WOMAN's photo,based on a MAN's photo(condition)<br/>
discriminators X : to judge the MAN's photo, is it a fake one or real one?<br/>
discriminators y : to judge the WOMAN's photo, is it a fake one or real one?<br/>

Here's the training method:<br/>
1.real MAN-> gen x -> fake WOMAN -> dis y --> real or fake?<br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;-> gen y -> fake MAN' --> loss with real MAN?<br/>

2.real WOMAN->gen y -> fake MAN -> dis x --> real or fake?<br/>
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;-> gen x -> fake WOMAN' --> loss with real WOMAN?<br/>
                                
                                
