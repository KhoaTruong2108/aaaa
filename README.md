Chương 6. ƯỚC LƯỢNG THAM SỐ
§1. Ước lượng điểm
Ước lượng điểm bằng thống kê
a) Định nghĩa 1. Ước lượng điểm tham số M của đám đông X là dùng một thống kê G để thay thế cho M thỏa mãn một trong các tiêu chuẩn sau:
(1) Không chệch. Thống kê G gọi là ước lượng không chệch của tham số M nếu:
E
G
=
M
.
EG=M.

(2) Vững. Thống kê G gọi là ước lượng vững của tham số M nếu G hội tụ theo xác suất về M. Nghĩa là khi n đủ lớn thì xác suất P(G ≈ M) gần 1.
(3) Hiệu quả. Thống kê G gọi là ước lượng hiệu quả của tham số M nếu:
Không chệch: EG = M;
G có phương sai bé nhất trong các ước lượng không chệch của M.
b) Ước lượng điểm bằng các đặc trưng mẫu
Tham số của đám
đông	Ước lượng điểm
Tính chất ước lượng			
EX
=
µ	X¯	Không chệch; vững; hiệu quả		
p	f	Không chệch; vững; hiệu quả		
2
V
(X) =
σ	2
S
(phương sai mẫu)	Vững; bị chệch		
2
V
(X) =
σ	2
s
(phương sai mẫu
hiệu chỉnh)	Vững; không chệch		
c) Trong thực hành: Với kích thước mẫu n đủ lớn từ một mẫu cụ thể ta lấy:

μ
=
x
ˉ
,
p
=
f
=
k
n
,
σ
2
=
s
2
.
μ= 
x
ˉ
 ,p=f= 
n
k
​
 ,σ 
2
 =s 
2
 .

Ví dụ 1.
Điều tra chiều cao một loại giống cây trồng trong khoảng thời gian T cho kết quả:

Chiều cao (cm)	30–40	40–50	50–60	60–70	70–80	80–90	90–100
Số cây	4	18	26	35	20	12	5
1

(a) Cây có chiều cao lớn hơn 70 cm là cây loại A. Hãy ước lượng tỷ lệ cây loại A.
(b) Hãy ước lượng chiều cao trung bình của các cây trồng.
(c) Hãy ước lượng phương sai của chiều cao giống cây trồng.
2. Ước lượng điểm bằng phương pháp mô men
Cho mẫu (x1, x2, . . . , xn) của đám đông X, ta gọi

m
k
=
1
n
∑
i
=
1
n
x
i
k
m 
k
​
 = 
n
1
​
 ∑ 
i=1
n
​
 x 
i
k
​
 

là mômen mẫu bậc k.

Sử dụng mk làm ước lượng của µk = E(Xk ) (mômen bậc k của đám đông X).

Phương pháp ước lượng bằng mômen: Cho đám đông X có hàm mật độ (liên tục) hay phân phối (rời rạc) là f(x, m), m là tham số của phân phối này. Ước lượng mômen bậc k của tham số m là nghiệm của hệ:

μ
1
=
m
1
,
⋯
 
,
μ
k
=
m
k
.
μ 
1
​
 =m 
1
​
 ,⋯,μ 
k
​
 =m 
k
​
 .

Ví dụ. Cho X ∼ P(λ). Từ mẫu (x1, . . . , xn) của đám đông X, ước lượng λ bằng phương pháp mômen.

3. Ước lượng điểm bằng phương pháp Hợp lí cực đại (Maximum likelihood)
Cho đám đông X có hàm mật độ (liên tục) hay phân phối (rời rạc) là f(x, m), m là tham số.

Lập hàm hợp lí từ mẫu (x1, x2, . . . , xn):

L
(
x
1
,
x
2
,
…
,
x
n
;
m
)
=
f
(
x
1
,
m
)
f
(
x
2
,
m
)
⋯
f
(
x
n
,
m
)
=
∏
j
=
1
n
f
(
x
j
,
m
)
.
L(x 
1
​
 ,x 
2
​
 ,…,x 
n
​
 ;m)=f(x 
1
​
 ,m)f(x 
2
​
 ,m)⋯f(x 
n
​
 ,m)=∏ 
j=1
n
​
 f(x 
j
​
 ,m). (1)

a) Định nghĩa 2. Giá trị mˆ được gọi là ước lượng hợp lí cực đại của tham số m (trên tập M) nếu:

L
(
x
1
,
…
,
x
n
;
m
^
)
=
max
⁡
m
∈
M
L
(
x
1
,
…
,
x
n
;
m
)
.
L(x 
1
​
 ,…,x 
n
​
 ; 
m
^
 )=max 
m∈M
​
 L(x 
1
​
 ,…,x 
n
​
 ;m). (2)

b) Tìm ước lượng hợp lí cực đại: Đặt x = (x1, . . . , xn), giả sử L(x, m) có đạo hàm đến cấp 2 theo m.

2

• Tìm điểm dừng bằng cách giải:

∂
L
(
x
,
m
)
∂
m
=
0.
a
g
3
∂m
∂L(x,m)
​
 =0.ag3

• Kiểm tra nghiệm của (3) để tìm cực đại.

Khẳng định: Giả sử (x1, . . . , xn) là mẫu cụ thể của đám đông X.

(i) Nếu X ∼ P(λ) thì ước lượng hợp lí cực đại của λ là x¯.
(ii) Nếu X ∼ N(µ, σ2 ) thì ước lượng hợp lí cực đại của µ là x¯, của σ 2 là S 2 .
§2. Ước lượng khoảng
1. Bài toán
Cho đám đông X có tham số M chưa biết, cho xác suất 1 − α tìm hai thống kê G1, G2 sao cho:

P
(
G
1
<
M
<
G
2
)
=
1
−
α
.
(
4
)
P(G 
1
​
 <M<G 
2
​
 )=1−α.(4)

Trong đó:

1
−
α
1−α là độ tin cậy, 
(
G
1
,
G
2
)
(G 
1
​
 ,G 
2
​
 ) là khoảng tin cậy.

Giải bài toán:
• Bước 1. Tìm thống kê G có phân phối xác suất xác định. Với xác suất 1 − α, tìm các phân vị gα/2 và g1−α/2 sao cho

P
(
G
>
g
α
/
2
)
=
α
2
,
P
(
G
>
g
1
−
α
/
2
)
=
1
−
α
2
.
P(G>g 
α/2
​
 )= 
2
α
​
 ,P(G>g 
1−α/2
​
 )=1− 
2
α
​
 .

• Bước 2. Từ khoảng (g1−α/2 < G < gα/2) biến đổi thành (G1 < M < G2).

2. Ước lượng khoảng của các tham số
Ước lượng tỉ lệ. a) Tóm tắt: Cho đám đông X có tỷ lệ p chưa biết. Cho độ tin cậy 1 − α, tìm khoảng tin cậy cho p.
Từ Định lí giới hạn trung tâm (Lindeberg–Levy), với n đủ lớn, lấy thống kê:

z = \frac{f - p}{\sqrt{\frac{f(1 - f)}{n}}} \approx N(0, 1). \tag{5}

Bài toán 1. Khoảng tin cậy đối xứng cho p:

p
∈
f
±
z
α
/
2
f
(
1
−
f
)
n
.
p∈f±z 
α/2
​
  
n
f(1−f)
​
 
​
 . (6)

Khoảng tin cậy một bên:

p
≤
f
+
z
α
f
(
1
−
f
)
n
p≤f+z 
α
​
  
n
f(1−f)
​
 
​
  hoặc 
p
≥
f
−
z
α
f
(
1
−
f
)
n
p≥f−z 
α
​
  
n
f(1−f)
​
 
​
  , 
(
1
−
α
=
Φ
(
z
α
)
)
(1−α=Φ(z 
α
​
 )) .

Bài toán 2. Từ ε = zα/2 r f(1 − f) n , suy ra kích thước mẫu cần điều tra:

n
≥
z
α
/
2
2
f
(
1
−
f
)
ε
2
.
(
7
)
n≥ 
ε 
2
 
z 
α/2
2
​
 f(1−f)
​
 .(7)

Chú ý: Khi cho độ tin cậy 1 − α và sai số ε thì

n
≥
0.25
 
z
α
/
2
2
ε
2
n≥0.25 
ε 
2
 
z 
α/2
2
​
 
​
 

thỏa mãn với tất cả các mẫu.

Bài toán 2.2. Cho sai số ε tìm độ tin cậy:

z
α
/
2
=
ε
n
f
(
1
−
f
)
,
1
−
α
2
=
Φ
(
z
α
/
2
)
,
z 
α/2
​
 =ε 
f(1−f)
n
​
 
​
 ,1− 
2
α
​
 =Φ(z 
α/2
​
 ),

nên

1
−
α
=
1
−
2
(
1
−
Φ
(
z
α
/
2
)
)
.
1−α=1−2(1−Φ(z 
α/2
​
 )).

Ví dụ 1. Kiểm tra ngẫu nhiên 500 sản phẩm thấy có 20 phế phẩm.

(a) Với độ tin cậy 96% ước lượng tỷ lệ phế phẩm.
(b) Với độ tin cậy 96% ước lượng tỷ lệ phế phẩm tối đa.
(c) Muốn độ tin cậy 98% và độ chính xác 1.5% thì cần điều tra thêm bao nhiêu sản phẩm.
(d) Muốn độ chính xác 1.5% thì độ tin cậy đạt được là bao nhiêu.
Ước lượng trung bình. Cho đám đông X có trung bình EX = µ chưa biết. Cho độ tin cậy 1 − α, tìm khoảng tin cậy cho µ.
Biết V (X) = σ 2 :
z
=
X
ˉ
−
μ
σ
/
n
∼
N
(
0
,
1
)
.
z= 
σ/ 
n
​
 
X
ˉ
 −μ
​
 ∼N(0,1).

• Chưa biết V (X), dùng s 2 :

t
=
X
ˉ
−
μ
s
/
n
∼
t
(
n
−
1
)
.
t= 
s/ 
n
​
 
X
ˉ
 −μ
​
 ∼t(n−1).

Khoảng tin cậy đối xứng:

μ
∈
x
ˉ
±
z
α
/
2
σ
n
,
μ
∈
x
ˉ
±
t
α
/
2
s
n
.
μ∈ 
x
ˉ
 ±z 
α/2
​
  
n
​
 
σ
​
 ,μ∈ 
x
ˉ
 ±t 
α/2
​
  
n
​
 
s
​
 .

Khoảng tin cậy một bên:

μ
≤
x
ˉ
+
z
α
σ
n
,
μ
≥
x
ˉ
−
z
α
σ
n
,
μ≤ 
x
ˉ
 +z 
α
​
  
n
​
 
σ
​
 ,μ≥ 
x
ˉ
 −z 
α
​
  
n
​
 
σ
​
 ,

hoặc (khi σ 2 chưa biết):

μ
≤
x
ˉ
+
t
α
s
n
,
μ
≥
x
ˉ
−
t
α
s
n
.
μ≤ 
x
ˉ
 +t 
α
​
  
n
​
 
s
​
 ,μ≥ 
x
ˉ
 −t 
α
​
  
n
​
 
s
​
 .

Chú ý: Trường hợp n ≥ 30, nếu X chuẩn, phương sai chưa biết có thể tra bảng chuẩn:

μ
∈
x
ˉ
±
z
α
/
2
s
n
.
μ∈ 
x
ˉ
 ±z 
α/2
​
  
n
​
 
s
​
 .

Ví dụ 2. Khảo sát nhu cầu (kg/tháng) của các hộ:

0
−
1
:
10
,
1
−
2
:
35
,
2
−
3
:
86
,
3
−
4
:
132
,
4
−
5
:
78
,
5
−
6
:
31
,
6
−
7
:
18
,
7
−
8
:
10.
0−1:10,1−2:35,2−3:86,3−4:132,4−5:78,5−6:31,6−7:18,7−8:10.

4

(1) Ước lượng nhu cầu trung bình với độ tin cậy 95%.
(2) Sai số không quá 0.12 kg/tháng, độ tin cậy 98% cần điều tra bao nhiêu hộ.
(3) Sai số không quá 0.12 kg/tháng thì độ tin cậy đạt được là bao nhiêu.
