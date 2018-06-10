---
layout: posts
title:  "Lí thuyết tập hợp - Quan hệ"
subtitle: "Quan hệ là gì?"
date:   2018-01-24
categories: [dai-so]
permalink:
cover:
description:
mathjax: true
---

## Mục tiêu

-  Quan hệ hai ngôi, quan hệ hai ngôi đồng nhất là gì?
-  Quan hệ ngược
-  Các tính chất có thể có của quan hệ hai ngôi
-  Hợp hai quan hệ
___

Đây đây tới cái phần hồi trước mình bắt đầu "xoắn não" đây =)). Quay lại về khái niệm tập hợp ở trên, khi nhắc đến tập hợp là tụi mình mới với về khái niệm "gom cái gì đó vào một chỗ", để "làm được gì đó" với tập hợp ta vẫn cần phải một _vài thứ khác_. Và đây khái niệm cơ bản khi học về cơ sở dữ liệu sau này.  Như ở bài trước, tụi mình đã định nghĩa về _quan hệ bao hàm_ nhưng chưa có gì đã định nghĩa về _Quan hệ_ cả. Do đó trong phần này tụi mình sẽ tìm hiểu về _quan hệ_, và chủ yếu là _quan hệ hai ngôi_. Tại sao gọi là _quan hệ hai ngôi_? =)) đơn giản là quan hệ giữa hai vật nào đó. Nhưng mình đã nói từ tập hợp chúng ta sẽ có được nhiều thứ, và bây giờ tụi mình sẽ xây dựng _quan hệ hai ngôi_ từ thứ tụi mình đang có: Tập hợp.

## Quan hệ (hai ngôi) là gì?

>$$E,\,F$$ là hai tập hợp. Mọi bộ ba $$(E,\,\Gamma,\, F)$$, trong đó $$\Gamma \in \mathfrak{P}(E \times F)$$, gọi là quan hệ từ $$E$$ đến $$F$$. Cho $$x \in E$$ và $$y \in F$$, nếu $$x$$ có quan hệ $$\mathcal{R}$$ với $$y$$ thì $$(x,y) \in \Gamma$$.

Tụi mình có thể kí hiệu $$x\mathcal{R}y$$ thay cho $$(x,y)\in \Gamma$$.<br/>
$$E$$ gọi là tập nguồn của $$\mathcal{R}$$. $$x \in E$$ <br/>
$$F$$ gọi là tập đích của $$\mathcal{R}$$. $$y \in F$$<br />
$$\Gamma$$ gọi là đồ thị của $$\mathcal{R}$$. <br />

**Chú ý**: khi $$F = E$$ thì ta gọi $$\mathcal{R}$$ là **quan hệ hai ngôi** đồng nhất. Đây là khái niệm quan hệ phổ biến trong toán học.

Bản thân mình thấy định nghĩa trên khá phức tạp, nhưng nó lại khá chặt chẽ vì khi định nghĩa quan hệ, sau này là hàm, phần lớn sẽ quên định nghĩa tập nguồn và tập đích của quan hệ. Từ định nghĩa trên, tụi mình có thể hiểu việc định nghĩa quan hệ dựa trên bộ ba $$E,\Gamma, F$$ là giúp chúng ta luôn nhớ định nghĩa tập nguồn và tập đích của quan hệ. $$\Gamma$$ là tập hợp các $$(x,y) \in E \times F$$ có quan hệ $$\mathcal{R}$$ với nhau. Vậy ta có thể hiểu định nghĩa quan hệ mang tính "tập hợp" hơn.

Quan hệ là tập hợp các cặp có thứ tự $$(x,y) \in E \times F$$ mà các tập nguồn $$E$$ và tập đích $$F$$ được xác định rõ. Như vậy, quan hệ vẫn chỉ là tập hợp nhé, không có gì lạ lẫm hết =)).

Từ đó ta viết các quan hệ $$\in, \subset$$ nhìn có vẻ "toán" hơn =)).

  $$\in\,  = (E, \,\Gamma,\, \mathfrak{P}(E) )$$. $$\Gamma = \{(x,A): x \, \text{thuộc}\, A\}$$.

Chú ý là tập hợp $$E$$ ở đây không giống như ở trên định nghĩa mà là tập hợp trừu tượng được coi là chứa tất cả mọi thứ. Nhớ lại tụi mình không có định nghĩa là khái niệm "thuộc", mà chỉ chấp nhận nó. Nếu $$x \in E, A\in \mathfrak{P}(E), x\in A \Rightarrow (x,A) \in \Gamma $$.


Từ đây, ta có thể định nghĩa quan hệ bao hàm của hai tập hợp. $$\subset \, = (E,\Gamma,E)$$, $$ \Gamma = \{(A,B) : \forall x \in A \Rightarrow x \in B  \}$$.


Ví dụ: Chúng ta chưa đề cập đến tập số nguyên, nhưng trong ví dụ này sẽ coi như các bạn đã "biết" về tập hợp số nguyên rồi.
  Quan hệ "bé hơn" trong tập hợp số nguyên: $$<\, = (\mathbb{Z}, \Gamma, \mathbb{Z}) $$ với $$\Gamma = {(x,y) : x < y}$$. Việc làm sao để biết $$x < y$$ thì các bạn sẽ biết khi học về tập hợp số nguyên. Do $$3 < 5 \Rightarrow (3,5) \in \Gamma$$ của $$<$$.

Ví dụ khác: Ta có thể biễu diễn một quan hệ bằng biểu đồ hình tên, trong đó mũi tên sẽ đi từ $$x$$ đến $$y$$ để mô tả $$x\mathcal{R}y$$.

![Ví dụ về quan hệ](../../images/post2/img_2.svg)

Dựa vào biểu đồ trên, tụi mình có đồ thị $$\Gamma$$ của $$\mathcal(R)$$ là $$\Gamma= \{(Nam,Lan), (Nam,Trang),(Thành,Trang),(Long,Mai)\}$$. Để ý là chiều của mũi tên chỉ có từ $$E$$ đến $$F$$, điều đó nhắc lại cho tụi mình là đồ thị của quan hệ được định nghĩa từ những cặp có thứ tự, khi nói về quan hệ ta chỉ mang tính "một chiều" từ tập đích đến tập nguồn. Điều đó có nghĩa là Nam "thích" Trang nhưng ngược lại Trang "thích" Nam thì chưa chắc. Các bạn nam cũng nên nhớ điều này =)).

Từ đây, tụi mình có thể định nghĩa **quan hệ n ngôi** như sau: <br />

>Với $$E_1, E_2, ..., E_n$$ là những tập hợp. Quan hệ n ngôi là một bộ (n+1) $$(E_1,E_2,...,E_n,\Gamma)$$. Với $$\Gamma \in \mathfrak{P}(E_1 \times E_2 ... \times E_n)$$. <br/>

**Chú ý:** Nếu các bạn để ý thì ở phần định nghĩa quan hệ hai ngôi ở trên thì mình có thêm chữ "đồng nhất", điều này có nghĩa là
tập đích bằng tập nguồn.


Một vài ví dụ về quan hệ


Quan hệ 3 ngôi: Để diễn tả một quan hệ, trước hết, tụi mình định nghĩa 3 tập hợp như sau: tập hợp 3 chàng trai $$E = \{Dũng,\, Thanh,\, Chinh\}$$, tập hợp 3 cô gái $$F = \{Đào,\, Mai,\, Phượng\}$$, tập họp 4 món quà $$G=\{Hoa,\, Gấu,\, Kẹo,\, Bánh\}$$.
Ta có bộ 3 $$(Dũng,\, Đào,\, Gấu)$$ diễn tả quan hệ 3 ngôi Dũng tặng Đào bằng Gấu. Quan hệ 3 ngôi được dùng khi không thể diễn tả trực tiếp quan hệ giữa các phần tử của các tập hợp. Tương tự đối với các quan hệ n-ngôi khác. Tương tự ví dụ này, ta có ví dụ: Một giáo viên dạy học sinh trong một lớp học nào đó chẳng hạn.


Hoặc một ví dụ về toán học, với một quan hệ $$\mathcal{R} = (\mathbb{Z},\, \mathbb{Z},\, \mathbb{Z},\, \Lambda)$$ với một bộ ba số nguyên $$(a,\,b,\,c) \in \Gamma$$ thì $$ a < b < c$$. Vậy $$(1,2,3) \in \Gamma$$, $$(2,1,3) \notin \Gamma$$.


Hay cái danh sách học sinh của tụi mình chính là một ví dụ cho quan hệ n-ngôi.

![Ví dụ quan hệ n-ngôi](../../images/post2/img_1.png)

Vậy là tụi mình đã biết được $$x$$ có quan hệ với $$y$$, vậy thì $$y$$ có quan hệ gì với $$x$$? Từ đó, ta bắt đầu nghĩ đến khái niệm _quan hệ ngược_.


## Quan hệ ngược
$$E,F$$ là hai tập hợp, $$\mathcal{R}$$ là một quan hệ từ $$E$$ đến $$F$$. Quan hệ ngược của $$\mathcal{R}$$, kí hiệu $$\mathcal{R}^{-1}$$, là quan hệ từ $$F$$ đến $$E$$, được định nghĩa bởi:
> $$\forall (x,y) \in E \times F, y \mathcal{R}^{-1} x \Leftrightarrow x\mathcal{R}y$$

Định nghĩa trên có nghĩa là gì? Kí hiệu $$\Leftrightarrow$$ ở đây chỉ phép toán logic "tương đương". Mệnh đề $$A \Leftrightarrow B $$ là đúng khi hai mệnh đề A,B cùng đúng hoặc cùng sai. Ở đây, $$ y \mathcal{R}^{-1} x \Leftrightarrow x\mathcal{R}y $$ có nghĩa là khi  $$ y \mathcal{R}^{-1} x $$ đúng, mà khi nào thì $$ y \mathcal{R}^{-1} x $$ đúng? Đó là khi cặp $$(y,x)$$ thuộc đồ thị của $$\mathcal{R}^{-1}$$. Khi  $$ y \mathcal{R}^{-1} x $$ đúng thì $$ x\mathcal{R}y $$ đúng điều này có nghĩa là $$(x,y)$$ thuộc đồ thị của $$\mathcal{R}$$. Vậy tóm gọn lại là $$ y \mathcal{R}^{-1} x \Leftrightarrow x\mathcal{R}y$$ có nghĩa khi tụi mình có quan hệ $$x\mathcal{R}y$$ thì cặp $$(y,x)$$ thuộc đồ thị của $$\mathcal{R}^{-1}$$ sẽ cho tụi mình định nghĩa về quan hệ $$\mathcal{R}^{-1}$$.


**Ví dụ**

'<' là quan hệ 2 ngôi ngược với quan hệ '>' trong $$\mathbb{N}$$. <br/>
Quan hệ có $$\Gamma = \{(1,A), (2,B), (3,C)\}$$ là quan hệ ngược đối với quan hệ có $$\Gamma=\{(A,1), (B,2), (C,3)\}$$ với E là tập hợp chữ số, F là tập hợp chữ cái. <br/>

**Chú ý:**

 Với mỗi quan hệ bất kì, sẽ luôn tồn tại quan hệ ngược đối với nó.


## Các tính chất mà quan hệ hai ngôi có thể có

Một quan hệ hai ngôi $$\mathcal{R}$$ trong một tập hợp $$E$$ được gọi là:

**phản xạ** khi và chỉ khi: $$\forall x \in E, x\mathcal{R}x$$

**đối xứng** khi và chỉ khi: $$\forall (x,y) \in E^2, x\mathcal{R}y \Rightarrow y\mathcal{R}x $$

**phản đối xứng** khi và chỉ khi: $$\forall (x,y) \in E^2, \begin{cases} x\mathcal{R}y \\ y\mathcal{R}x \end{cases} \Rightarrow x = y $$

**bắc cầu** khi và chỉ khi: $$\forall (x,y,z) \in E^3, \begin{cases} x\mathcal{R}y \\ y\mathcal{R}z \end{cases} \Rightarrow x\mathcal{R}z $$


Oh trời, một loạt tính chất răn mà nhớ nỗi trời, thực ra mình nghĩ các bạn bây giờ không cần phải thuộc các khái niệm trên, chỉ cần đọc đi đọc lại vài lần là quen thôi. Và mình chú ý là các tính chất trên không phải tất cả quan hệ hai ngôi nào cũng có. Vậy tại sao cần phải biết nó? vì không phải quan hệ hai ngôi nào cũng có tất cả các tính chất trên nên ta có thể dùng các tính chất trên để phân biệt các quan hệ với nhau.


**Ví dụ**

phản xạ: trong tập E là tập hợp loài người thì quan hệ "thích" có tính phản xạ. Vì mình nghĩ, tất cả mọi người, ai có cũng "thích" bản thân mình hết.


Một chút toán hơn, quan hệ bao hàm $$\subset$$ trong tập hợp $$E$$ chứa tất cả các tập hợp có tính phản xạ, $$A\subset A$$, vì $$\forall x \in A \Rightarrow x \in A$$ =)).


đối xứng: quan hệ '=' trong tập hợp số nguyên.


phản đối xứng: quan hệ $$\le$$ trong tập hợp số tự nhiên.


bắc cầu: quan hệ 'song song' của 2 đường thẳng trong một mặt phẳng. Hay quan hệ 'là họ hàng ruột' trong tập hợp loài người.  


Tại sao nó giúp chúng ta phân biệt quan hệ?


So sánh hai quan hệ $$\in$$ và $$\subset$$, thấy quan hệ $$\in$$ không có tính phản xạ và bắc cầu, ta có đưa ra một phản ví dụ: tập hợp các số nguyên $$\mathbb{Z} = \{...,-1,0,1,...\}$$, ta có thể thấy $$\mathbb{Z}$$ không phải là phần tử của $$\mathbb{Z}$$. Quan hệ $$\in$$ không có tính bắc cầu,
ta cũng có một phản ví dụ: $$3\in \mathbb{Z} \wedge \mathbb{Z} \in A =\{\mathbb{Z}, \mathbb{Q}, \mathbb{R}\}$$ nhưng $$3 \notin A$$. Trong khi đó, quan hệ $$\subset$$ lại có tính phản xạ và bắc cầu. <br/>
Hay trong tập hợp loài người, coi trong tập hợp này mỗi người chỉ được làm một công việc. Ta có quan hệ "là đồng nghiệp" là quan hệ có tính bắt cầu. Còn quan hệ "là người yêu" thì không có tính bắc cầu =)). À mà, nãy giờ lấy ví dụ là về quan hệ hai ngôi nhé các bạn.


Và các bạn có thể để thấy các ví dụ nãy giờ của mình về quan hệ luôn nhắc đến tập đích và tập nguồn của quan hệ. <br/>
Trước khi về một vài loại quan hệ "đặc biệt" thì tụi mình hãy nói về kiểu quan hệ 'lồng ghép' vào nhau. Kiểu như bạn có quan hệ 'là bạn trai' đối với Phương. Quang có quan hệ 'là người yêu cũ' đối với Phương. Vậy, Bạn có quan hệ gì đối với Quang?<br/>
Từ bài toán kiểu như thế, ta nghĩ đến khái niệm về  quan hệ hợp.


## Quan hệ hợp
$$E,F,G$$ là các tập hợp. $$\mathcal{R}$$ là một quan hệ từ $$E$$ đến $$F$$. $$\mathcal{S}$$ là một quan hệ từ $$F$$ đến $$G$$. Quan hệ hợp của $$\mathcal{R}$$ và $$\mathcal{S}$$, kí hiệu $$\mathcal{S}\circ \mathcal{R}$$, là quan hệ từ $$E$$ đến $$G$$ được xác định bởi:

> $$\forall (x,z) \in E \times G, \, x \mathcal{S} \circ \mathcal{R} z \Leftrightarrow \exists y \in F, \begin{cases} x \mathcal{R} y \\ y \mathcal{S} z \end{cases} $$

**Ví dụ:**

Lấy lại 3 tập hợp E,F,G ở phần quan hệ 3 ngôi ở trên: $$E = \{Dũng,\, Thanh,\, Chinh\}$$, $$F = \{Đào,\, Mai,\, Phượng\}$$, $$G=\{Hoa,\, Gấu,\, Kẹo,\, Bánh\}$$. $$\mathcal{R}$$ là quan hệ "là bạn trai" từ E đến F. $$\mathcal{S}$$ là quan hệ "thích" từ F đến G. Vậy quan hệ "mua" từ E đến G chính là quan hệ hợp $$S \circ R$$

Không biết các bạn có giống mình không lúc đầu cái kí hiệu $$\mathcal{S} \circ \mathcal{R}$$ cảm thấy nó bị ngược ngược răn á =)). Sau ni mình mới để ý là bọn mình sẽ định nghĩ hàm từ quan hệ, và tụi mình cũng sẽ có khái niệm <i>hàm hợp</i>.
Giống như quan hệ hợp, nếu như tụi mình có 2 hàm f, g thì hàm hợp sẽ được kí hiệu: $$f \circ g$$, khi đó ta sẽ có: $$x g \circ f z$$, cái này viết lại $$z = g\circ f(x) = g(f(x))$$. Và cái gì trong ngoặc sẽ thực hiện trước đúng không nào? Nghĩa là
f sẽ "tác động" lên x trước sau đó đến g "tác động" lên f(x). Như vậy, sẽ thấy 'thuận thuận' đúng không? Và việc viết g trước f sẽ không thay đổi thứ tự khi ta thay đổi cách viết hàm hợp. Do đó, việc viết $$\mathcal{S}$$ trước $$\mathcal{R}$$, sẽ
cũng có nghĩa chúng ta sẽ quan tâm đến quan hệ $$x\mathcal{R}y$$ trước quan hệ $$y\mathcal{S}z$$. Vì quan hệ hợp vẫn là quan hệ nên nó vẫn là một tập hợp và quan hệ hợp có đồ thị $$\Gamma = \{(x,z): \exists y \in F, \begin{cases} x \mathcal{R} y \\ y \mathcal{S} z \end{cases} \}$$  


Và một trong những điều lưu ý đối với quan hệ hợp là quan hệ ngược đối với một quan hệ hợp.<br/>


## Quan hệ ngược của một quan hệ hợp
$$E,F,G$$ là các tập hợp. $$\mathcal{R}$$ là một quan hệ từ $$E$$ đến $$F$$. $$\mathcal{S}$$ là một quan hệ từ $$F$$ đến $$G$$. Ta có:
>$$(\mathcal{S} \circ \mathcal{R})^{-1} = \mathcal{R}^{-1} \circ \mathcal{S}^{-1}$$

**Chứng minh**

$$\forall (x,z) \in E \times G$$:

$$z(\mathcal{S}\circ\mathcal{R})^{-1} \Leftrightarrow x\mathcal{S} \circ \mathcal{R} z \Leftrightarrow \exists y \in F: \begin{cases} x\mathcal{R}y \\ y\mathcal{S}z\end{cases} \Leftrightarrow
\exists y \in F, \begin{cases} z\mathcal{S}^{-1}y \\ y\mathcal{R}^{-1}x\end{cases} \Leftrightarrow \mathcal{R}^{-1} \circ \mathcal{S}^{-1}$$

Cũng hơi dài rồi nên để các nội dung còn lại sang bài viết khác. Chúc các bạn vững bước trên con đường của mình.

## Tham khảo

Đại số 1 - Jean-Marie Monier <br/>
Giáo trình toán - thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
Elements of Set Theory - Herbert B. Enderton<br/>
[N-ary relationship types - vertabelo.com](http://www.vertabelo.com/blog/technical-articles/n-ary-relationship-types)
