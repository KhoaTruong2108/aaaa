# Chương 6. ƯỚC LƯỢNG THAM SỐ

## §1. Ước lượng điểm

### 1. Ước lượng điểm bằng thống kê

#### a) Định nghĩa

**Định nghĩa 1.**  
Ước lượng điểm tham số \( M \) của đám đông \( X \) là dùng một thống kê \( G \) để thay thế cho \( M \), thỏa mãn một trong các tiêu chuẩn sau:

1. **Không chệch**  
   \( G \) gọi là ước lượng không chệch của \( M \) nếu:
   \[
   E(G) = M
   \]

2. **Vững**  
   \( G \) gọi là ước lượng vững của \( M \) nếu \( G \) hội tụ theo xác suất về \( M \), tức là khi \( n \) đủ lớn:
   \[
   P(G \approx M) \to 1
   \]

3. **Hiệu quả**  
   \( G \) gọi là ước lượng hiệu quả của \( M \) nếu:
   - \( E(G) = M \) (không chệch);
   - \( G \) có phương sai nhỏ nhất trong các ước lượng không chệch của \( M \).

---

### b) Ước lượng điểm bằng các đặc trưng mẫu

| Tham số của đám đông | Ước lượng điểm | Tính chất |
|---------------------|----------------|-----------|
| \( E(X) = \mu \) | \( \bar{X} \) | Không chệch; vững; hiệu quả |
| \( p \) | \( f \) | Không chệch; vững; hiệu quả |
| \( V(X) = \sigma^2 \) | \( S^2 \) (phương sai mẫu) | Vững; bị chệch |
| \( V(X) = \sigma^2 \) | \( s^2 \) (phương sai mẫu hiệu chỉnh) | Vững; không chệch |

---

### c) Trong thực hành

Với kích thước mẫu \( n \) đủ lớn, ta lấy:
\[
\mu = \bar{x}, \quad p = f = \frac{k}{n}, \quad \sigma^2 = s^2
\]

---

### Ví dụ 1

Điều tra chiều cao cây trồng thu được kết quả:

| Chiều cao (cm) | 30–40 | 40–50 | 50–60 | 60–70 | 70–80 | 80–90 | 90–100 |
|---------------|------|------|------|------|------|------|-------|
| Số cây | 4 | 18 | 26 | 35 | 20 | 12 | 5 |

Yêu cầu:
1. Ước lượng tỷ lệ cây cao hơn 70 cm (loại A).
2. Ước lượng chiều cao trung bình.
3. Ước lượng phương sai chiều cao.

---

## 2. Ước lượng điểm bằng phương pháp mô men

Cho mẫu \( (x_1, x_2, \ldots, x_n) \), mômen mẫu bậc \( k \):

\[
m_k = \frac{1}{n} \sum_{i=1}^{n} x_i^k
\]

Dùng \( m_k \) để ước lượng:
\[
\mu_k = E(X^k)
\]

**Phương pháp mô men:**  
Nếu phân phối của \( X \) là \( f(x, m) \), ước lượng tham số \( m \) bằng nghiệm của hệ:
\[
\mu_1 = m_1,\; \mu_2 = m_2,\; \ldots,\; \mu_k = m_k
\]

**Ví dụ:**  
Nếu \( X \sim P(\lambda) \) thì:
\[
\hat{\lambda} = \bar{x}
\]

---

## 3. Ước lượng điểm bằng phương pháp Hợp lí cực đại (MLE)

Hàm hợp lí:
\[
L(x_1,\ldots,x_n;m) = \prod_{j=1}^{n} f(x_j,m)
\]

**Định nghĩa 2.**  
\( \hat{m} \) là ước lượng hợp lí cực đại nếu:
\[
L(x;\hat{m}) = \max_{m \in M} L(x;m)
\]

**Cách tìm:**
- Giải:
\[
\frac{\partial L(x,m)}{\partial m} = 0
\]
- Kiểm tra cực đại.

**Kết quả chuẩn:**
- Nếu \( X \sim P(\lambda) \): \( \hat{\lambda} = \bar{x} \)
- Nếu \( X \sim N(\mu,\sigma^2) \):
  \[
  \hat{\mu} = \bar{x}, \quad \hat{\sigma}^2 = S^2
  \]

---

## §2. Ước lượng khoảng

### 1. Bài toán

Tìm \( G_1, G_2 \) sao cho:
\[
P(G_1 < M < G_2) = 1 - \alpha
\]

- \( 1-\alpha \): độ tin cậy  
- \( (G_1, G_2) \): khoảng tin cậy

---

### 2. Ước lượng khoảng tỉ lệ \( p \)

Với mẫu lớn:
\[
z = \frac{f - p}{\sqrt{\frac{f(1-f)}{n}}} \sim N(0,1)
\]

**Khoảng đối xứng:**
\[
p \in f \pm z_{\alpha/2} \sqrt{\frac{f(1-f)}{n}}
\]

**Khoảng một bên:**
\[
p \le f + z_\alpha \sqrt{\frac{f(1-f)}{n}}
\quad \text{hoặc} \quad
p \ge f - z_\alpha \sqrt{\frac{f(1-f)}{n}}
\]

**Cỡ mẫu cần thiết:**
\[
n \ge \frac{z_{\alpha/2}^2 f(1-f)}{\varepsilon^2}
\]

Trường hợp xấu nhất:
\[
n \ge \frac{0.25\, z_{\alpha/2}^2}{\varepsilon^2}
\]

---

### Ví dụ 1

Kiểm tra 500 sản phẩm, có 20 phế phẩm:

1. Khoảng tin cậy 96% cho tỷ lệ phế phẩm.
2. Tỷ lệ phế phẩm tối đa (96%).
3. Với độ tin cậy 98% và sai số 1.5%, cần khảo sát thêm bao nhiêu sản phẩm?
4. Với sai số 1.5%, độ tin cậy đạt được là bao nhiêu?

---

### 3. Ước lượng trung bình \( \mu \)

- **Biết \( \sigma^2 \):**
\[
z = \frac{\bar{X} - \mu}{\sigma/\sqrt{n}} \sim N(0,1)
\]

- **Chưa biết \( \sigma^2 \):**
\[
t = \frac{\bar{X} - \mu}{s/\sqrt{n}} \sim t(n-1)
\]

**Khoảng đối xứng:**
\[
\mu \in \bar{x} \pm z_{\alpha/2}\frac{\sigma}{\sqrt{n}}
\quad \text{hoặc} \quad
\mu \in \bar{x} \pm t_{\alpha/2}\frac{s}{\sqrt{n}}
\]

---

### Ví dụ 2

Khảo sát nhu cầu (kg/tháng):

| Khoảng | 0–1 | 1–2 | 2–3 | 3–4 | 4–5 | 5–6 | 6–7 | 7–8 |
|------|----|----|----|----|----|----|----|----|
| Số hộ | 10 | 35 | 86 | 132 | 78 | 31 | 18 | 10 |

Yêu cầu:
1. Ước lượng nhu cầu trung bình (95%).
2. Sai số ≤ 0.12 kg, độ tin cậy 98% ⇒ cần bao nhiêu hộ?
3. Sai số ≤ 0.12 kg ⇒ độ tin cậy đạt được là bao nhiêu?
