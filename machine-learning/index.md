# machine learning study (Coursera)

# Model and Cost function
Model
```
 x_i -> h -> y_i
input        output

(h: hypothesis)
```
Cost function
```
J(theta_0, theta_1) = 1/2m * sum[1 to m](y_i^ - y_i)^2
```

# Gradient Descent
기울기가 낮은 쪽으로 local minimum을 찾아가는 경사 하강법
```diff
theta_1 := theta_1 - alpha * d/d*theta_1 J(theta_1)

alpha따라
too small:
    slow하게 내려감
too large:
    converge하거나 diverge

@@ for linear regression @@
converge까지 repeat {
    theta_0 := theta_0 - alpha * 1/m sum[1 to m](h_theta(x_i) - y_i)
    theta_1 := theta_1 - alpha * 1/m sum[1 to m]((h_theta(x_i) - y_i) * x_i)
}
```


