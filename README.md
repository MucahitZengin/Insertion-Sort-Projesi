Insertion Sort Projesi
======================
[22,27,16,2,18,6] -> Insertion Sort

# Adımlar:
* [22,27,16,2,18,6]
<br>&nbsp;^ &emsp; &emsp;&nbsp;&nbsp;^ 
* [**2**,27,16,22,18,6]

* [**2**,27,16,22,18,6]
<br>&emsp;^&emsp;&emsp;&emsp;&emsp;&nbsp; ^
* [**2**,**6**,16,22,18,27]

* [**2**,**6**,16,22,18,27]
<br>&emsp;&emsp;^
* [**2**,**6**,**16**,22,18,27]

* [**2**,**6**,**16**,22,18,27]
<br>&emsp;&emsp;&emsp;^&emsp;^
* [**2**,**6**,**16**,**18**,22,27]

* [**2**,**6**,**16**,**18**,22,27]
<br>&emsp;&emsp;&emsp;&emsp;&nbsp;^  
* [**2**,**6**,**16**,**18**,**22**,27]

* [**2**,**6**,**16**,**18**,**22**,27]
<br>&emsp;&emsp;&emsp;&emsp;&emsp;&nbsp;&nbsp;^
* [**2**,**6**,**16**,**18**,**22**,**27**]

# Big-O:
Önce hepsini tarayıp en küçüğü baştakiyle değiştirir. (n adım)
Sonra ilk eleman hariç tüm elemanları tarayıp ikinci indisteki elemanla değiştirir. (n-1 adım)
Bu şekilde son elemana kadar gelir.(1 adım) 
> n+(n-1)+(n-2)+...+1
>
> =(n*(n+1))/2
>
> =(n^2)/2+n/2     (en büyük değişken dışındaki değişkenler yoksayılır)
>
> =(n^2)/2         (katsayılar yoksayılır)
>
> = n^2

Big-O karmaşıklık katsayısı **O(n^2)**'dir.