Insertion Sort Projesi
======================
# Soru 1: [22,27,16,2,18,6] -> Insertion Sort
## Adımlar:
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

## Big-O:
Önce hepsini tarayıp en küçüğü baştakiyle değiştirir. (n adım)

Sonra ilk eleman hariç tüm elemanları tarayıp ikinci indisteki elemanla değiştirir. (n-1 adım)

Bu şekilde son elemana kadar gelir.(1 adım) 
> n+(n-1)+(n-2)+...+1
>
> =(n*(n+1))/2
>
> =(n<sup>2</sup>)/2+n/2     (en büyük değişken dışındaki değişkenler yoksayılır)
>
> =(n<sup>2</sup>)/2         (katsayılar yoksayılır)
>
> = n<sup>2</sup>

Big-O zaman karmaşıklığı **O(n<sup>2</sup>)**'dir.

## Time Complexity:
**Best case(n<sup>2</sup>):** Sıralıdır. Yer değiştirme olmasa da yine n<sup>2</sup> tarama yapılır.

**Worst cese(n<sup>2</sup>):** Tüm elemanlar sıralı halindeki konumundan farklı bir konumdadır. Ama hepsi tarandığı için zaman karmaşıklığı n<sup>2</sup>'dir.

**Average case(n<sup>2</sup>):** Best case ile worst case eşit olduğundan average case de n<sup>2</sup>'dir.

## 18 sayısı
Dizi sıralandıktan sonra 18 sayısı average case kapsamına girer.

# Soru 2: [7,3,5,8,2,9,4,15,6] dizisinin ilk 4 adımı
1. [7,3,5,8,2,9,4,15,6]
<br>&nbsp;^&emsp;&emsp;&nbsp;^
2. [**2**,3,5,8,7,9,4,15,6]

3. [**2**,3,5,8,7,9,4,15,6]
<br>&emsp;^
4. [**2**,**3**,5,8,7,9,4,15,6]
