<div>
<h1>Insertion Sort</h1>
<table>

<tr>  <th>Adım</th>  <th>Dizi Durumu</th>  </tr>

<tr>  <td>1.</td> ->  <td>[22,27,16,2,18,6]</td>  </tr>

<tr>  <td>2.</td>  ->  <td>[22,27,16,2,18,6]</td>  </tr>

<tr>  <td>3.</td> ->   <td>[16,22,27,2,18,6]</td>  </tr>

<tr>  <td>4.</td>  ->  <td>[2,16,22,27,18,6]</td>  </tr>

<tr>  <td>5.</td> ->   <td>[2,16,18,22,27,6]</td>  </tr>

<tr>  <td>6.</td>  ->  <td>[2,6,16,18,22,27]</td>  </tr>

</table>

<h2>Insertion Sort - Big-O Gösterimi ve Zaman Karmaşıklığı</h2>

<p>Insertion Sort, bir dizi elemanını küçükten büyüğe (ya da büyükten küçüğe) sıralamak için kullanılan bir algoritmadır. En kötü durumda, Insertion Sort'un zaman karmaşıklığı <b>O(n^2) 'dir.</b> Bu, sıralanacak eleman sayısının karesi kadar işlem yapılması anlamına gelir. Ortalama durumda da Insertion Sort'un zaman karmaşıklığı O(n^2) 'dir. Ancak, bazı özel durumlarda (örneğin, n elemanlı bir dizinin zaten sıralı olduğu durumda) Insertion Sort'un zaman karmaşıklığı daha düşük olabilir.</p>
</div>

<div>
<br>----------------------------

<h2>Selection Sort</h2>

<p>Selection Sort, bir dizi elemanını küçükten büyüğe (ya da büyükten küçüğe) sıralamak için kullanılan bir algoritmadır. Algoritma, en küçük elemanı seçerek ilk pozisyona yerleştirir, ardından ikinci en küçük elemanı seçerek ikinci pozisyona yerleştirir ve bu şekilde devam eder.</p>

<h3>Dizi</h3>

<p>[7,3,5,8,2,9,4,15,6]</p>

<hr>

<h3>1. Adım</h3>

<p>En küçük eleman 2 olduğundan, 2 ile ilk eleman yer değiştirir:</p>

<p>[<b>2</b>,3,5,8,7,9,4,15,6]</p>

<hr>

<h3>2. Adım</h3>

<p>En küçük 2.eleman 3 olduğundan yer değiştirmez </p>

<p>[2,<b>3</b>,5,8,7,9,4,15,6]</p>

<hr>

<h3>3. Adım</h3>

<p>En küçük 3. sayı 4 olduğu için 4 ile 5 yer değişir</p>

<p>[2,3,<b>4</b>,8,7,9,5,15,6]</p>

<hr>

<h3>4. Adım</h3>

<p>En küçük 4. sayı 5 olduğu için 5 ile 8 yer değişir</p>

<p>[2,3,4,<b>5</b>,7,9,8,15,6]</p>

</div>
<br>----------------------------

<h2>Merge Sort</h2>
<p>İlk olarak, verilen diziyi Merge Sort algoritmasına göre sıralayalım.</p>
<ol>
<li><p>Dizi elemanlarını yarıya bölelim:
[16,21,11] ve [8,12,22]</p></li>
<li><p>Her bir alt dizi için tekrar yarıya bölelim:
[16], [21,11] ve [8], [12,22]</p></li
><li><p>Her bir alt-alt dizi için tek eleman kalana kadar yarıya bölelim:
[16], [21], [11] ve [8], [12], [22]</p></li>
<li><p>Her alt-alt dizi için sıralayarak birleştirelim:
[16], [11,21] ve [8], [12,22]</p></li>
<li><p>İki alt dizi için de birleştirme işlemi yapalım:
[11,16,21] ve [8,12,22]</p></li>
<li><p>Son olarak, iki alt diziyi birleştirerek tam sıralı diziyi elde edelim:
[8,11,12,16,21,22]</p></li>
</ol>
<p>Böylece, verilen dizi Merge Sort algoritmasına göre sıralanmıştır.</p>
<p>Big-O gösterimi için, Merge Sort algoritması <b>O(nlogn)</b> zamanda çalışır. Bu nlogn terimi, algoritmanın çalışma süresinin n elemanlı diziler için logaritmik bir artış göstermesinden kaynaklanır. Bu durum, Merge Sort'un genellikle hızlı ve verimli bir sıralama algoritması olarak tercih edilmesine sebep olur.</p>

<br>----------------------------
<h2>Binary Search Tree</h2>
<p>Başlangıçta boş bir ağaç ile başlayalım ve verilen dizi elemanlarını sırayla ekleyelim. Binary-Search-Tree özelliğine göre, her düğümde sol alt ağaçtaki tüm elemanlar o düğümden küçük ve sağ alt ağaçtaki tüm elemanlar o düğümden büyük olacak şekilde düzenleyeceğiz.</p>
<p><b>Dizimiz : </b> [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]</p>
<p><b>1.)</b> 7 düğümünü kök olarak ekleyin.</p>
<p><b>2.)</b> 5 düğümü, 7'den küçük olduğu için sol alt ağaca ekleyin. </p>
<p><b>3.)</b> 1 düğümü, 7'den küçük olduğu için sol alt ağacın soluna ekleyin.</p>
<p><b>4.)</b> 8 düğümü, 7'den büyük olduğu için sağ alt ağaca ekleyin. </p>
<p><b>5.)</b> 3 düğümü, 5'ten küçük olduğu için sol alt ağacın soluna ekleyin.</p>
<p><b>6.)</b> 6 düğümü, 5'ten büyük ve 7'den küçük olduğu için sol alt ağaca ekleyin.</p>
<p><b>7.)</b> 0 düğümü, 7'den küçük olduğu için sol alt ağacın soluna ekleyin.</p>
<p><b>8.)</b> 9 düğümü, 7'den büyük olduğu için sağ alt ağaca ekleyin.</p>
<p><b>9.)</b> 4 düğümü, 5'ten büyük ve 7'den küçük olduğu için sol alt ağaca ekleyin.</p>
<p><b>10.)</b> 2 düğümü, 5'ten küçük olduğu için sol alt ağacın sağ altına ekleyin.</p>
<p><b>Bu şekilde, verilen dizinin Binary-Search-Tree'deki aşamaları Aşağıdaki şekildedir.</b></p>

                      7
		         / \
                    5   8
                   / \   \
                  1   3   9
                 / \     
	            0   4	
		       /
                  2
		      
<br>----------------------------
<p><b>Bu Proje Patika.dev # Başlangıç Seviyesi .Net Core Patikası Eğitim için yaptığım # Veri Yapıları ve Algoritmalar Projesi için yapılmıştır </b></p>
