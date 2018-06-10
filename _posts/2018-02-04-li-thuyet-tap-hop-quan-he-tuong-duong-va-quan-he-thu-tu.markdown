---
layout: posts
title:  "Lí thuyết tập hợp - Quan hệ tương đương và quan hệ thứ tự"
subtitle: "Hai loại quan hệ phổ biến"
date:   2018-02-4
categories: [dai-so]
permalink:
cover:
description:
mathjax: true


---

## Mục tiêu

-  Hai loại quan hệ phổ biến
-  Quan hệ tương đương
-  Quan hệ thứ tự

___

## Hai loại quan hệ phổ biến

Như trong bài viết về quan hệ, tụi mình đã biết các tính chất có thể có của một quan hệ là: phản xạ, đối xứng, phản đối xứng và bắc cầu. Vậy, bây giờ tụi mình sẽ cùng nhau tìm hiểu về hai loại quan hệ phổ biến: quan hệ tương đương và quan hệ thứ tự. Tại sao hai quan hệ này lại phổ biến? Từ đầu đến giờ, tụi mình đã liên tục nhắc lại một thứ đó là: Tập hợp. Mọi thứ tụi mình làm việc xung quanh đều là tập hợp đúng không nào? Tập hợp có thể là tập hợp số, hàm số, tập hợp quần áo, tập hợp nhân viên trong một công ty, ... Và để nguyên các tập hợp như vậy thì tụi mình vẫn chưa "làm việc" được gì đúng không nào? Để làm việc được thì tụi mình phải định nghĩa các "phép toán" : cộng, trừ, nhân, chia, ... chi đó, điều này tụi mình sẽ cùng nhau nhắc đến sau ở phần các cấu trúc đại số. Thay vào đó, trước tiên, trong toán học, cũng như các công việc hằng ngày, tụi mình cần phải biết cách "phân loại", "sắp xếp", để công việc của tụi mình có thể thực hiện được và thực hiện có hiệu quả.

Để có thể thực hiện được "phép cộng" trên tập hợp số tự nhiên, tụi mình phải sắp xếp các số tự nhiên lên trên một "tia số" hay "trục số", rồi việc thực hiện "phép cộng" chỉ là việc "dịch chuyển" vị trí trên "trục số" đó thôi. Ví dụ: để thực hiện "phép cộng" 0 với 1 trên tập hợp các số tự nhiên thì tụi mình chỉ cần dịch chuyển từ vị trí 0 lên 1 đơn vị trên trục số. Do đó, tụi mình có thể thấy, nếu không "sắp xếp" các số tự nhiên trên "trục số" thì lỡ 2 ở vị trí của 1 thì "phép cộng" 0 + 1 sẽ trở thành 0 + 1 = 2.

Hay công việc hằng ngày, tụi mình cũng phải "sắp xếp" các công việc theo một "thứ tự" ưu tiên, hay phân loại quần áo, loại nào mặc ấm, loại nào mặc đi chơi ...

Khi thực hiện "phân loại" hay "sắp xếp" tụi mình đều cần có các loại quan hệ như quan hệ tương đương và quan hệ thứ tự. Đương nhiên, trong cuộc sống hằng ngày, tụi mình không cần phải hiểu đến mức "cặn kẽ" các khái niệm toán học thì mới có thể "sắp xếp" hay "phân loại" được công việc của tụi mình. Nhưng việc hiểu các khái niệm này sẽ hiểu thấu đáo được các nguyên lí làm việc trong các vấn đề kĩ thuật sau này và cũng giúp tụi mình suy nghĩ một cách có logic hơn.

Vậy, hãy xem thử quan hệ tương đương và quan hệ thứ tự là gì nhé.

## Quan hệ tương đương

> Quan hệ tương đương $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất" trên tập hợp F và có các tính chất: phản xạ, đối xứng, bắc cầu.

**Ví dụ**

- Quan hệ bằng nhau là quan hệ tương đương trong tập hợp các số tự nhiên. Vì:
  - Có tính phản xạ: $$\forall x \in \mathbb{N} : x = x$$
  - Có tính đối xứng: $$\forall (x,y) \in \mathbb{N}^2 : x = y \Rightarrow y = x$$
  - Có tính bắc cầu: $$\forall (x,y,z) \in \mathbb{N}^3 : x = y \, \text{và}\, y = z \Rightarrow x = z$$

- Quan hệ song song trong tập hợp các đường thẳng thuộc cùng một mặt phẳng $$D$$ là quan hệ tương đương. Vì:
  - Có tính phản xạ: $$\forall a \in D : a \parallel a $$
  - Có tính đối xứng: $$\forall (a,b) \in D^2 : a \parallel b \Rightarrow b \parallel a $$
  - Có tính bắc cầu: $$\forall (a,b,c) \in D^3 : a \parallel b \, \text{và}\, b \parallel c \Rightarrow a \parallel c $$

- Quan hệ "ở trong cùng một gia đình" trong tập hợp loài người H là quan hệ tương đương. Vì:
  - Có tính phản xạ: $$\forall a \in H : a \,\text{ở trong cùng một gia đình với}\, a $$. Ví dụ: Lan ở trong cùng một gia đình với Lan.
  - Có tính đối xứng: $$\forall a \in H^2 : a \,\text{ở trong cùng một gia đình với}\, b \Rightarrow b \,\text{ở trong cùng một gia đình với}\, a $$
  - Có tính bắc cầu: $$\forall (a,b,c) \in H^3 : a $$ ở trong cùng một gia đình với $$ b $$ và $$ b $$ ở trong cùng một gia đình với $$ c \Rightarrow a $$ ở trong cùng một gia đình với $$c $$.

**Chú ý**

- Trong bài viết này, tụi mình sẽ chỉ nói về định nghĩa quan hệ tương đương, quan hệ thứ tự, các quan hệ này có tính chất như thế nào, chứ không phải là thực hiện việc "so sánh" hay "phân loại" các phần tử. Khi thực hiện việc "so sánh", tụi mình cần phải có một "tiêu chuẩn" nào đó.

Trong cuộc sống hằng ngày, khi "so sánh" mức độ quan trọng của một công việc, tụi mình có thể dựa vào tiêu chuẩn là khoảng cách thời gian từ bây giờ đến thời hạn. Nếu khoảng thời gian từ bây giờ đến thời hạn của công việc này ngắn hơn khoảng thời gian từ bây giờ đến thời hạn của công việc kia thì công việc này sẽ "quan trọng hơn" công việc kia.

Hay khi hai số tự nhiên với nhau chính là tụi mình đang dựa vào khoảng cách từ vị trí của mỗi số đến điểm số 0. Hay trong việc phân loại các bài viết trong vào chủ đề, tụi mình sẽ dựa vào "tiêu chuẩn" là "độ liên quan" của mỗi bài viết đến các chủ đề. Quan hệ "ở trong cùng một chủ đề" là quan hệ tương đương dựa trên "tiêu chuẩn" là độ liên quan" của mỗi bài viết đến các chủ đề.

Trong toán học, tụi mình cũng có các tiêu chuẩn như vậy, được gọi dưới cái tên là "chuẩn". Khái niệm "chuẩn" tụi mình sẽ cùng nhau nói ở những phần tiếp theo. Khi đi sâu vào kĩ thuật, các bạn sẽ có thể định nghĩa các "chuẩn" của riêng mình để cho công việc được hiệu quả hơn.


Tiếp theo, bây giờ tụi mình có tập hợp và các phần tử của nó, cùng với quan hệ hai ngôi đồng nhất được định nghĩa trên tập hợp đó. Khi làm việc với phần tử $$x$$ của tập hợp, sẽ có lúc tụi mình cần xem những phần tử nào có quan hệ với x. Để biết một số nào đó có  chia hết cho 3 hay không trong tập hợp các số tự nhiên, tụi mình sẽ quan tâm đến tập hợp các số có quan hệ "là bội" đối với 3. Hay trong tập loài người, nếu tổ chức nào đó muốn làm việc với bạn, ví dụ như trường học, chẳng hạn, thì có thể họ sẽ quan tâm đến tập hợp những ai có quan hệ "trong cùng gia đình" với bạn. Hay bạn có bao giờ quan tâm đến tập hợp những ai có quan hệ "là người yêu thương, lo lắng" cho bạn? Vì nhu cầu trên, tụi mình sẽ có khái niệm về lớp tương đương.


### Lớp tương đương
> $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất" trong tập hợp $$F$$. Với mọi $$x$$ thuộc $$F$$, lớp tương đương của $$x$$ là tập hợp, kí hiệu: $$cl_\mathcal{R}(x)$$ được xác định bởi:
> ## $$cl_\mathcal{R}(x) = \{ y \in E; x \mathcal{R} y \}$$

Hiểu là tập hợp các phần tử có quan hệ với $$x$$.

**Chú ý**
- $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất", không nhất thiết là quan hệ tương đương.
- Tụi mình biết $$x$$ là gì thì mới định nghĩa được tập hợp trên. Hay lớp tương đương được xác định với mỗi $$x$$.
- Cái này lúc mình hay bị lẫn lộn, mọi người chú ý quan hệ tương đương khác với toán tử tương đương $$\Leftrightarrow$$.


**Ví dụ**
- Cho một quan hệ tương đương $$\mathcal{R}$$ có đồ thị $$\Gamma = \{(a,a), (b,b), (c,c), (b,c), (c,b)\}$$ định nghĩa trong tập hợp $$F=\{a,b,c\}$$, có thể ban đầu sẽ hơi thắc mắc vì sao quan hệ trên là quan hệ tương đương?

Thứ nhất, quan hệ trên là quan hệ hai ngôi đồng nhất vì đồ thị của nó là tập hợp các cặp có thứ tự.
Thứ hai, quan hệ trên có các tính chất: phản xạ, đối xứng, bắc cầu.<br/>
Tính phản xạ: $$\forall x \in F, x\mathcal{R}y$$, vì các cặp $$(a,a), (b,b), (c,c) \in \Gamma$$ suy ra $$a\mathcal{R}a,\,b\mathcal{R}b,\,c\mathcal{R}c$$.

Tính đối xứng: $$\forall (x,y) \in F^2, x \mathcal{R}y \Rightarrow y\mathcal{R}x$$, vì dựa vào đồ thị $$\Gamma$$, ta thấy:

 $$a \mathcal{R}a \Rightarrow a\mathcal{R}a$$ vì $$(a,a) \in \Gamma$$

 $$b \mathcal{R}b \Rightarrow b\mathcal{R}b$$ vì $$(b,b) \in \Gamma$$

$$c \mathcal{R}c \Rightarrow c\mathcal{R}c$$ vì $$(c,c) \in \Gamma$$

$$b \mathcal{R}c \Rightarrow c\mathcal{R}b$$ vì $$(b,c), (c,b)\in \Gamma$$

 Chắc sẽ có bạn thắc mắc vì sao không có $$a\mathcal{R}b$$ - ban đầu, mình cũng từng thắc mắc - điều này đơn giản là vì $$(a,b) \notin \Gamma$$

Tính bắc cầu:

$$ c \mathcal{R} b \, \text{và}\, b \mathcal{R} c \Rightarrow c \mathcal{R} c $$. Do $$(c,b), (b,c), (c,c) \in \Gamma$$

$$ b \mathcal{R} c \, \text{và}\, c \mathcal{R} b \Rightarrow b \mathcal{R} b$$. Do $$(b,c), (c,b), (b,b) \in \Gamma$$

Vậy $$\mathcal{R}$$ là quan hệ tương đương trong $$F$$.

Tụi mình có, đối với $$a$$, tập hợp các phần tử thuộc $$F$$ có quan hệ $$\mathcal{R}$$ với $$a$$ là $$\{a\}$$. Suy ra, $$cl_\mathcal{R}(a)=\{a\}$$.

 đối với $$b$$, tập hợp các phần tử thuộc $$F$$ có quan hệ $$\mathcal{R}$$ với $$b$$ là $$\{b,c\}$$. Suy ra, $$cl_\mathcal{R}(b)=\{b,c\}$$. Tương tự đối với $$c$$.


- Trong tập hợp loài người, thì mỗi gia đình là một lớp tương đương của một người đối với quan hệ "ở trong cùng một gia đình".

- Danh sách bạn bè trên Facebook của bạn là một lớp tương đương của bạn đối với quan hệ "là bạn bè trên Facebook"

- Danh sách crush của bạn là một lớp tương đương của bạn đối với quan hệ "là người thầm thương, trộm nhớ". Trong trường hợp này $$\mathcal{R}$$ chỉ là quan hệ hai ngôi.

### Tập thương
>Tập thương của E bởi $$\mathcal{R}$$, kí hiệu là $$E/\mathcal{R}$$, là tập hợp các lớp tương đương đối với quan hệ $$\mathcal{R}. $$
> $$ E/\mathcal{R}=\{cl_{\mathcal{R}}(x) : x \in E\}$$

**Ví dụ**

- Lấy ví dụ đầu tiên ở trên, tụi mình sẽ có $$E/\mathcal{R} = \{\{a\},\{b,c\}\}$$

**Chú ý**

- Đối với $$x,y$$ khác nhau và cùng thuộc một tập hợp $$E$$, $$\mathcal{R}$$ là quan hệ tương đương trong $$E$$, thì một là $$cl_\mathcal{R}(x) \cap cl_\mathcal{R}(y) = \varnothing$$ hoặc hai là  $$cl_\mathcal{R}(x) = cl_\mathcal{R}(y) $$


Chứng minh:

Nếu $$cl_\mathcal{R}(x) \cap cl_\mathcal{R}(y) \neq \varnothing$$

Giả sử: $$z \in cl_\mathcal{R}(x) \cap cl_\mathcal{R}(y) \Rightarrow  \begin{cases} x\mathcal{R}z \\ y\mathcal{R}z \end{cases} \Rightarrow \begin{cases} x\mathcal{R}z \\ z\mathcal{R}y  \end{cases} \Rightarrow x\mathcal{R}y $$. Do $$\mathcal{R}$$ là quan hệ tương đương.

Với $$\forall t \in cl_\mathcal{R}(x) \Rightarrow x\mathcal{R}t \Rightarrow t\mathcal{R}x$$

 Vì $$ \begin{cases} t\mathcal{R}x \\ x\mathcal{R}y \end{cases} \Rightarrow t\mathcal{R}y \Rightarrow y\mathcal{R}t \Rightarrow  t \in cl_\mathcal{R}(y)$$

Vậy, $$\forall t \in cl_\mathcal{R}(x) \Rightarrow t \in cl_\mathcal{R}(y)$$ nên $$cl_\mathcal{R}(x) \subset cl_\mathcal{R}(y)$$

Tương tự, cho chiều ngược lại, tụi mình chứng minh dược $$cl_\mathcal{R}(y) \subset cl_\mathcal{R}(x)$$

Do đó, $$cl_\mathcal{R}(y) =  cl_\mathcal{R}(x)$$


Tiếp theo, tụi mình sẽ đến với loại quan hệ phổ biến thứ hai là quan hệ thứ tự. Quan hệ thứ tự RẤT quan trọng vì khi định nghĩa được "thứ tự" từ đó tụi mình mới có thể sắp xếp, thực hiện các công việc được hiệu quả, cũng như quan hệ thứ tự có ý nghĩa quan trọng trong việc hiểu các bài toán cực trị hay các bài toán tối ưu. Các bài toán quan trọng trong Machine Learning.



# Quan hệ thứ tự
> Quan hệ thứ tự $$\mathcal{R}$$ là một quan hệ hai ngôi "đồng nhất" từ tập hợp F và có các tính chất: phản xạ, phản đối xứng, bắc cầu.

**Chú ý**
- Quan hệ thứ tự thường được kí hiệu là $$\preceq$$ thay cho $$\mathcal{R}$$.

- Hai phần tử gọi là so sánh được khi có quan hệ thứ tự giữa hai phần tử này.

- Một tập hợp $$E$$ cùng với một quan hệ thứ tự $$\preceq$$ được định nghĩa trong nó tạo thành cặp $$(E, \preceq)$$ gọi là một tập hợp được sắp thứ tự.

- Vì các phần tử của tập hợp không nhất thiết phải là số, nên quan hệ thứ tự không nhất thiết phải mang nghĩa thứ tự thông thường như đối với các số. Thứ tự ở đây có thể có ý nghĩa về "gần - xa", "lớn - trẻ", "trước - sau", "trên - dưới", "giống - khác".

- $$\preceq$$ là một **quan hệ thứ tự toàn phần** khi và chỉ khi mọi phần tử của E đều so sánh được với nhau từng đôi.

**Ví dụ**
- Quan hệ $$\leq$$ thông thường trong tập hợp các số tự nhiên là quan hệ thứ tự toàn phần. Vì có:
  - Tính phản xạ. $$\forall x \in \mathbb{N}, x \leq x$$. Ví dụ: $$1 \leq 1$$
  - Tính phản đối xứng. $$\forall (x,y) \in \mathbb{N}^2, \begin{cases} x \leq y \\ y \leq x \end{cases} \Rightarrow x = y $$. Ví dụ: $$ a \leq 0 $$ và $$ 0 \leq a $$ suy ra $$a = 0$$.
  - Tính bắc cầu. $$ \forall (x,y,z) \in \mathbb{N}^3, \begin{cases} x \leq y \\ y \leq z \end{cases}  \Rightarrow x \leq z$$


- Quan hệ bao hàm $$\subset$$ là quan hệ thứ tự không toàn phần trong $$\mathfrak{P}(E)$$ với E là tập hơp có nhiều hơn hai phần tử.

Giả sử $$E=\{1,2\} \Rightarrow \mathfrak{P}(E)=\{\varnothing, \{1\}, \{2\}, \{1,2\}\}$$. Tụi mình có: $$\varnothing \subset \{1\}, \, \varnothing \subset \{2\}, \, \varnothing \subset \{1,2\}, \, \{1\} \subset \{1,2\}, \{2\} \subset \{1,2\}$$ nhưng $$\{1\} \not\subset \{2\}$$


- Quan hệ "chia hết" là quan hệ thứ tự không toàn phần trong tập hợp các số tự nhiên.


- Quan hệ "là hậu duệ" trong tập hợp con người không phải quan hệ thứ tự vì không có tính phản xạ thay vào đó nó được gọi là quan hệ thứ tự "nghiêm ngặt".


- Quan hệ "đến sớm hơn" là một quan hệ thứ tự trong tập hợp là một hàng người đang chờ để mua hàng.


- Quan hệ "xa hơn" dựa trên cách một điểm nào đó một bán kính $$R$$ là một quan hệ thứ tự không toàn phần. Vì các điểm trên cùng một mặt cầu không thể so sánh.


- Quan hệ "tốt hơn" trên tập hợp các học sinh trong một lớp được khi học lực và hạnh kiểm của học sinh này đều "lớn hơn" học sinh kia là một quan hệ thứ tự không toàn phần nếu xảy ra trường hợp học lực của học sinh này "lớn hơn" học sinh kia nhưng hạnh kiểm của học sinh này lại "kém hơn" học sinh kia.
Đây là ví dụ về (quan hệ) thứ tự tích được định nghĩa như sau:
Cho $$(E,\preceq)$$,$$(F,\preceq')$$ là hai tập hợp được sắp thứ tự. $$\mathcal{P}$$ là quan hệ xác định trong $$E\times F$$ bởi:

<center> $$(x,y)\mathcal{P}(x',y')\Leftrightarrow \begin{cases} x \preceq x' \\ y \preceq' y'  \end{cases}$$</center>


- Quan hệ thứ tự xuất hiện các từ trong từ điển là quan hệ thứ tự. (Quan hệ) thứ tự này được gọi là thứ tự từ điển. Được dùng phổ biến trong từ điển =)), trong các bảng xếp hạng, để so sánh trong các chuỗi trong một ngôn ngữ lập trình nào đó người ta cũng dựa vào thứ tự này. Thứ tự từ điển được định nghĩa như sau, coi mỗi phần tử cần chỉ có 2 "chỉ số" để so sánh:
Cho $$(E,\preceq)$$,$$(F,\preceq')$$ là hai tập hợp được sắp thứ tự. $$\mathcal{L}$$ là quan hệ xác định trên $$E\times F$$ bởi:

 $$(x,y)\mathcal{L}(x',y')\Leftrightarrow \Big\lbrack\begin{align} x \preceq x' \\ x = x' \, \text{và} \,y \preceq' y'  \end{align}$$


Qua một loạt ví dụ vừa rồi, mình chỉ muốn nhấn mạnh quan hệ thứ tự ở đây không nhất thiết phải là quan hệ thứ tự thông thường giữa các số. Vì điều này làm mình luẩn quẩn một thời gian.

Bây giờ, mình nghĩ cái mà tụi mình khá quen thuộc đó chính là quan hệ thứ tự toàn phần. Cái rắc rối ở đây chính là quan hệ thứ tự không toàn phần. Vì như những ví dụ ở trên các bạn có thể thấy thứ tự không toàn phần khá phổ biến phải không nào? Thứ tự không toàn còn xuất hiện trong lí thuyết đồ thị có ứng dụng lớn trong việc giải quyết các bài toán phức tạp trong đời sống. Vì vậy, để làm việc, tụi mình cần thêm những khái niệm mới.


### Các phần tử đặc biệt trong tập hợp được sắp thứ tự
Các bạn lưu ý nhé, hãy nắm thật rõ các khái niệm này vì tụi mình sẽ gặp nó liên tục.

Trong các định nghĩa sau, tụi sẽ coi $$(E, \preceq)$$ là một tập hợp được sắp thứ tự.

#### Chặn trên và chặn dưới

##### Chặn trên

$$A\in \mathfrak{P}(E), x\in E$$. $$x$$ là một chặn trên hay cận trên của A trong $$E$$ khi và chỉ khi:
> ## $$\forall a \in A, a \preceq x $$

##### Chặn dưới

$$A\in \mathfrak{P}(E), x\in E$$. $$x$$ là một chặn dưới hay cận dưới của A trong $$E$$ khi và chỉ khi:
> ## $$\forall a \in A, x \preceq a $$

Tập hợp các chặn trên của $$A$$ trong $$E$$ là $$Maj_E(A)$$. Tập hợp các chặn dưới của $$A$$ trong $$E$$ là $$Min_E(A)$$. Các bạn nhớ các kí hiệu này vì sau này thay vì viết $$x$$ là cận trên của $$A$$ trong $$E$$, người ta hay viết $$x \in Maj_E(A)$$. Tương tự với cận dưới. Maj là từ viết tắt của "majorant" trong tiếng Pháp nghĩa là chặn trên, Min là từ viết tắt của "minorant" có nghĩa là chặn dưới.


Điều mình thắc mắc đầu tiên đó chính là tại sao không xét quan hệ thứ tự trên tập hợp $$E$$ luôn đi mà phải xét tới tập hợp con $$A$$ của $$E$$? Là do khi làm việc thì tụi mình chỉ làm việc với tập hợp con của một tập hợp lớn. Ví dụ: khi giáo viên muốn làm việc với lớp thì chỉ thường làm việc với ban cán sự lớp. Khi tìm từ "Hair" trong từ điển, tụi mình trong mục "H" ở đâu? hay cụ thể hơn là chữ đầu tiên bắt đầu bằng "H" và chữ cuối cùng kết thúc bằng "H" là ở vị trí nào.



**Chú ý**
- $$A$$ là tập hợp con của $$E$$. $$A$$ bị chặn trên (tương ứng: bị chặn dưới) khi và chỉ khi A có ít nhất một chặn trên (tương ứng: chặn dưới) trong $$E$$.

- Để ý là $$x\in E $$ nên $$x$$ có thể có hoặc không thuộc $$A$$, điều này giúp tụi mình phân biệt được với các khái niệm tiếp theo là cực trị và phần tử lớn nhất, nhỏ nhất.

- Một tập hợp có thể có nhiều cận trên và cận dưới hoặc không có cận trên hoặc cận dưới nào.


**Ví dụ**
- Coi Việt Nam là một hợp con trên Trái Đất. Chỉ xét theo chiều từ Bắc đến Nam thì những điểm có vĩ độ lớn hơn Lũng Cú (cực bắc Việt Nam) là chặn trên của Việt Nam. Những điểm ở thấp hơn về phía Nam đối với Mũi Cà Mau (cực Nam Việt Nam) là chặn dưới của Việt Nam.


- Đặt một tờ giấy trên mặt bàn, coi tờ giấy là một tập hợp con của mặt bàn, xét quan hệ thứ tự dọc theo chiều dài tờ giấy, thì cận trên của tờ giấy là tất cả các điểm "nằm trên" mép trên của tờ giấy, cận dưới của tờ giấy là tất cả các điểm "nằm dưới" mép dưới tờ giấy.


- Xét một hàng người như hình vẽ, xét quan hệ thứ tự từ phải sang trái, tập hợp gồm có {A,B,C,D} là tập con của hàng người trên. Tập hợp này có cận trên là A, và cận dưới là tất cả những người xếp sau D. (Cái hình chữ coi như cái bàn thu ngân, vẽ thêm cho đẹp thôi nhé.)

![Ví dụ về tập hợp sắp thứ tự](../../images/post3/img_1.png)

- Hình ảnh ví dụ về cận trên, nguồn: Wikipedia
![Ví dụ về  cận trên và cận dưới 1](../../images/post3/img_2.png)

- Một ví dụ về thứ tự không toàn phần. Đây là hình ảnh một cái cây, tụi mình sẽ cho cái cây một quan hệ thứ tự về độ cao, và mỗi nút trên cây có quan hệ thứ tự hay so sánh được khi chúng được nối với nhau như hình vẽ (các bạn có thể thấy không phải nút nào cũng có quan hệ thứ tự, cái đường thẳng ngang ở phía dưới hiểu là mặt đất nhé, chứ không có ý nghĩa gì nhiều đâu :v). Chiều của mũi tên chỉ chiều của quan hệ thứ tự. Từ hình vẽ, bạn có thể thấy,
  - Cận dưới của tập hợp $$\{6,7,8\}$$ là $$1, 6, 0$$ và tập hợp không có cận trên.

  - Tập hợp $$\{6,7\}$$ có cận dưới là $$1, 6, 0$$, cận trên là tất cả các nút "lớn hơn" $$7$$

  - Tập hợp $$\{0,1,7,8\}$$ không có cận trên và cận dưới.

![Ví dụ về cận trên và cận dưới 2](../../images/post3/img_3.png)

##### Biên trên
> Biên trên hay cận trên đúng là chặn trên thấp nhất.

Kí hiệu là $$Sup_E(A)$$ - Các bạn nhớ kí hiệu này nhé, hay quên lắm. Sup là từ viết tắt của từ Supremum trong tiếng anh và Borne Supérieure trong tiếng Pháp có nghĩa là biên trên.


##### Biên dưới
> Biên dưới hay cận dưới đúng là chặn dưới lớn nhất.

Kí hiệu là $$Inf_E(A)$$. Inf là viết tắt của từ Infimum trong tiếng anh và Borne Inférieure trong tiếng Pháp có nghĩa là biên dưới.

**Chú ý**
- Biên trên và biên dưới là duy nhất.

**Ví dụ**
- $$E = \mathfrak{P}(F)$$, $$F$$ là một tập hợp, quan hệ bao hàm $$\subset$$ là quan hệ thứ tự trong $$E$$. Với mọi $$(X,Y) \in E^2$$.

$$Sup_E(\{X,Y\}) = X \cup Y$$ và $$Inf_E(\{X,Y\}) = X \cap Y$$

- Hình ảnh mình lấy trên wikipedia ở phía trên có thể hiện biên trên.

- Ở ví dụ với cái cây ở trên, tập hợp $$\{6,7,7\}$$ có cận dưới nhưng không có cận dưới đúng.


### Phần tử lớn nhất, phần tử nhỏ nhất

#### Phần tử lớn nhất
>$$A \in \mathfrak{P}(E)$$. $$x$$ là phần tử lớn nhất của $$A$$ khi và chỉ khi:
> $$\begin{cases} x \in A \\ \forall a \in A, a \preceq x  \end{cases}$$

#### Phần tử nhỏ nhất
>$$A \in \mathfrak{P}(E)$$. $$x$$ là phần tử nhỏ nhất của $$A$$ khi và chỉ khi:
> $$\begin{cases} x \in A \\ \forall a \in A, x \preceq a  \end{cases}$$

**Chú ý**
- Để là phần tử lớn nhất hoặc nhỏ nhất thì $$x$$ phải là phần tử của $$A$$.

- Phần tử lớn nhất hoặc nhỏ nhất nếu tồn tại thì là duy nhất.

Chứng minh:

$$A \in \mathfrak{P}(E)$$. Cho $$x, x'$$ là hai phần tử nhất của $$A$$. Suy ra, $$x, x'$$ đều thuộc $$A$$ và $$x, x'$$ "lớn hơn hoặc bằng" tất cả các phần tử thuộc A. Nên $$\begin{cases} x \preceq x' \\ x' \preceq x \end{cases} \Rightarrow x = x'$$ (tính chất phản đối xứng).

- Khi cận trên đúng hoặc cận dưới đúng thuộc $$A$$ thì chúng sẽ là phần tử lớn nhất hoặc phần tử nhỏ nhất của $$A$$ theo như định nghĩa về phần tử lớn nhất và phần tử nhỏ nhất.


**Ví dụ**
- Cho tập hợp $$\{1,2,3\}$$ là tập con của tập hợp các số tự nhiên, có quan hệ thứ tự thông thường $$\leq$$. Tụi mình có phần tử lớn nhất là 3, phần tử nhỏ nhất là 1.

- Tiếp tục với ví dụ cái cây, tập hợp $$\{0,1,6\}$$ có quan hệ thứ tự được định nghĩa như hình vẽ có phần tử lớn nhất là 6 và không có phần tử nhỏ nhất.


### Phần tử cực đại, phần tử cực tiểu

#### Phần tử cực đại
> $$ A \in \mathfrak{P}(E), x \in A$$. $$x$$ là phần tử cực đại của $$A$$ khi và chỉ khi:
> $$ \forall a \in A, x \preceq a \Rightarrow x = a$$

#### Phần tử cực tiểu
> $$ A \in \mathfrak{P}(E), x \in A$$. $$x$$ là phần tử cực đại của $$A$$ khi và chỉ khi:
> $$ \forall a \in A, x \preceq a \Rightarrow x = a$$

Thú thật, lúc đầu học mình cũng không hiểu cái định nghĩa ni mô, mình không biết nó "cực đại" hay "cực tiểu" chỗ nào hết, và "cực đại" với "cực tiểu" thì khác chi "lớn nhất" với "nhỏ nhất".

Ta mình có hiểu là đối với phần tử cực đại $$x$$ thì không có phần tử nào "lớn hơn" nó và nếu có phần tử $$ y \in A$$ để có quan hệ thứ tự $$x \preceq y $$ thì chỉ mình $$x$$ mà thôi. Tương tự với phần tử cực tiểu.


**Chú ý**

- Khái niệm phần tử cực đại (cực tiểu) và phần tử lớn nhất (nhỏ nhất) là giống nhau đối với quan hệ thứ tự toàn phần.
- Có thể có nhiều phần tử cực đại hoặc cực tiểu.

**Ví dụ**
- Cho $$F = \{1,2,3\}. \mathfrak{P}(F) = \{\varnothing, \{1\}, \{2\},\{3\}, \{1,2\}, \{2,3\}, \{1,3\}, \{1,2,3\}\}$$. Quan hệ thứ tự ở đây là quan hệ bao hàm "x là tập con của y". Tụi mình có thể biểu diễn quan hệ thứ tự trên theo mỗi biểu đồ mũi tên như hình dưới.
  - Dựa vào biểu đồ, tụi mình có thể thấy, tập hợp $$A = \{\{1\},\{2\},\{3\},\{1,3\},\{1,2,3\}\}$$ có 3 phần tử cực tiểu là $$\{1\},\{2\},\{3\}$$ và 1 phần tử cực đại là $$\{1,2,3\}$$. Tại sao lại như vậy? Thì cứ theo định nghĩa, tụi mình sẽ suy ra được.
    - $$\{1\}$$ là phần tử cực tiểu, vì tụi mình có tìm trong tập hợp $$A$$ có phần tử $$a$$ nào để $$a \preceq \{1\}$$ không? Đáp án là chỉ là có $$\{1\}$$ thôi, $$\{1\}$$ chỉ tham gia vào quan hệ thứ tự trong $$\{1\} \preceq \{1\}, \{1\} \preceq \{1,3\}, \{1\} \preceq \{1,2,3\} \}$$. Xét trong tập hợp các quan hệ thứ tự của $$\{1\}$$, tụi mình có thể thấy $$\{1\}$$ không "lớn hơn" một phần tử nào cả, đó lí do tại sao nói là "cực tiểu". Mặc khác, để có phần tử $$y$$ nào thuộc $$A$$ để $$y\preceq \{1\}$$ thì chỉ có $$\{1\}$$ thôi, do đó không có có phần tử nào là "nhỏ hơn" $$\{1\}$$ nữa. Tương tự, các bạn có thể xem các trường hợp còn lại.  

![Ví dụ về cực trị 1](../../images/post3/img_4.png)

- Cho tập hợp $$E = \mathbb{N} - \{0,1\}$$ cùng với quan hệ thứ tự "là ước của" được định nghĩa trên nó. Xét tập con $$A = \{2,4,6\}$$. Quan hệ thứ tự của các phần tử trong $$A$$ có thể biểu diễn theo biểu đồ mũi tên như hình vẽ phía dưới. Dựa vào biểu đồ, tụi mình có thể thấy 2 vừa là phần tử nhỏ nhất, vừa là phần tử cực tiểu của tập hợp $$A$$. Tập hợp $$A$$ có 2 cực đại là 4 và 6. Tập A không có phần tử lớn nhất.

![Ví dụ về cực trị 2](../../images/post3/img_5.png)


Để tổng hợp lại những gì tụi mình vừa tìm hiểu, hãy làm một bài tập nhỏ coi như là một ví dụ cho tất cả các khái niệm ở trên.

Cho $$E = \{1,2,3,4,5\}, \mathcal{R}$$ là quan hệ thứ tự xác định trong $$E$$. Xét các tập con của $$E$$ là $$A = \{2,3\}, \, B = \{2,4\}, C = \{1,2,5\}$$. Quan hệ thứ tự được biểu diễn theo biểu đồ mũi tên. Hãy xem thử $$A,B,C$$ có phần tử lớn nhất, phần tử cực đại, biên trên hay không?

![Ví dụ về cực trị 3](../../images/post3/img_6.png)

Thay vì kí hiệu $$\mathcal{R}$$, tụi mình sẽ dùng $$\preceq$$ nhé.
Dựa vào biểu đồ này, tụi mình có các quan hệ, mình không liệt kê các quan hệ phản xạ như $$1\preceq 1$$ vào nhé: $$ 1 \preceq 2, 2 \preceq 5, 1\preceq 5, 1 \preceq 3, 3\preceq 5, 1 \preceq 4$$. Ở đây, các con số không phải là các số tự nhiên mà trừu tượng hoá của các đối tượng trong thực tế, ví dụ như các điạ điểm trên bản đồ chẳng hạn. Nên 2 không "nhỏ hơn" 3 hay 4 không "nhỏ hơn" 5 là hợp lí nhé (lúc đầu, mình không hiểu thật đó).

Đối với tập hợp $$A$$, tụi mình có các quan hệ: $$2\preceq 2, 3 \preceq 3$$. Tập hợp này có $$2, 3$$ là các phần tử cực đại cũng như là phần tử cực tiểu, không có giá trị lớn nhất, có biên trên là $$5$$.


Đối với tập hợp $$B$$, tụi mình có các quan hệ: $$2 \preceq 2, 4 \preceq 4$$. Tập hợp này không có biên trên vì chỉ có 2 là "nhỏ hơn" 5 còn 4 thì không, tương tự tập hợp $$A$$, $$2,4$$ vừa là phần tử cực đại vừa là phần tử cực tiểu của $$B$$. Tập hợp $$B$$ không có phần tử lớn nhất. Tập hợp B có biên dưới là 1.


Đối với tập hợp $$C$$, tụi mình có các quan hệ:  $$1 \preceq 1, 2 \preceq 2, 5 \preceq 5, 1 \preceq 2, 1\preceq 5, 2\preceq 5$$. Tập hợp $$C$$ có 5 vừa là phần tử lớn nhất, biên trên và phần tử cực đại, 1 vừa là phần tử nhỏ nhất vừa là phần tử cực tiểu.



Kết, hiểu được quan hệ tương đương và đặc biệt là quan hệ thứ tự sẽ giúp các bạn hiểu rõ được các bài toán sắp xếp, tối ưu, lí thuyết đồ thị cũng như các thuật toán "khó nhằng" trong lập trình, chúng đều là những bài toán ứng dụng thực tế cao. Bài viết hơi dài, hi vọng các bạn tìm thấy niềm vui trong việc khám phá ra những điều mới mẻ.


## Tham khảo

[Relations and their types - geeksforgeeks.org](https://www.geeksforgeeks.org/relations-and-their-types/)<br/>
[Equivalence relation - Wikipedia](https://en.wikipedia.org/wiki/Equivalence_relation)
[Equivalence class - Wikipedia](https://en.wikipedia.org/wiki/Equivalence_class)
[Order relation - Old Dominion University](http://www.cs.odu.edu/~cs381/cs381content/relation/order/order.html)<br/>
[Maximal and minimal elements - Wikipedia](https://en.wikipedia.org/wiki/Maximal_and_minimal_elements)<br/>
Đại số 1 - Jean-Marie Monier<br/>
Giáo trình Toán - Thầy Bùi Tuấn Khang<br/>
Naive Set Theory - Paul R. Halmos<br/>
Elements of Set Theory - Herbert B. Enderton<br/>
