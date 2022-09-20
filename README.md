# Lý thuyết
## 1. Dạng của Linear Regerssion
$$f_{\overrightarrow{w},b}(x)=\overrightarrow{w}x+b$$
Mô hình dự đoán: 
$$f_{\overrightarrow{w},b}(x^{(i)})=\overrightarrow{w}x^{(i)}+b$$
## 2. Hàm mất mát
$$J(W,b)=\frac{1}{2m} \sum\limits_{i=0}^{m}(f_{\overrightarrow{w},b}(x^{(i)})-y^{(i)})^2$$
## 3. Gradient Descent
$$b=b-\alpha\frac{\partial J(w,b)}{\partial b}$$
$$w_j=w_j-\alpha\frac{\partial J(w,b)}{\partial w_j}$$
$$
\frac{\partial J(w,b)}{\partial b}  = \frac{1}{m} \sum\limits_{i = 0}^{m-1} (f_{w,b}(x^{(i)}) - y^{(i)}) 
$$
$$
\frac{\partial J(w,b)}{\partial w_j}  = \frac{1}{m} \sum\limits_{i = 0}^{m-1} (f_{w,b}(x^{(i)}) -y^{(i)}).x^{(i)}_{j} 
$$

**Chú thích:**
* $f_{w,b}(x)$ : Hàm dự đoán.
* m: Số ví dụ.
* n: Số tính năng.
* $x^{(i)}$: Số ví dụ thứ i.
* $x^{(i)}_{j}$: Ví dự thứ i, tính năng thứ j.
* $\alpha$ : Tốc độ học tập.